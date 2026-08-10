Hood King Fanbase Signup — README


Overview


This project hosts a simple landing page for fans to join the Hood King community. The page collects name + email and saves signups into a Supabase Postgres table (FanBase). The site is intended to be deployed as a static site (GitHub Pages if public, or Netlify/Vercel if private).


What’s Included


Frontend: Static  index.html  landing page



Signup form fields:



 name  (required)



 email  (required)



Backend: Supabase Postgres table:  public."FanBase" 



Duplicate protection: Unique index on  lower(email) 



Security: Row Level Security (RLS) enabled with an insert-only policy for anonymous users



Requirements


A Supabase project



A Supabase table named FanBase with at least these columns:



 name  (text)



 email  (text)



(optional)  phone ,  interests ,  consent 



A deployed static site (GitHub Pages / Netlify / Vercel)



Supabase Setup


1) Confirm table name


In Supabase Table Editor, confirm the table is named FanBase (case-sensitive).


2) Prevent duplicate emails


Run in Supabase SQL Editor:



create unique index if not exists fanbase_email_unique
on public."FanBase" (lower(email));




3) Enable RLS + allow public inserts


Run in Supabase SQL Editor:



alter table public."FanBase" enable row level security;


drop policy if exists "Allow public insert" on public."FanBase";
create policy "Allow public insert"
on public."FanBase"
for insert
to anon
with check (true);




This allows anyone to submit the form, but does not allow anonymous users to read the fan list.


Frontend Configuration


1) Add Supabase client library


In  index.html   <head> :



<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>




2) Set Supabase URL + anon key


In the bottom  <script>  block of  index.html , set:


 SUPABASE_URL  to your Project URL (example:  https://xxxxx.supabase.co )



 SUPABASE_ANON_KEY  to your anon public key (JWT starting with  eyJ... )



Important:


Use the base project URL only (do not add  /rest/v1 ).



Never put the service role key in frontend code.



3) Insert into the correct table


Your JS should insert into:



.from("FanBase")




Deployment


Option A: GitHub Pages


Requires the repo to be public on free plans.



Ensure  index.html  is in the repo root.



Enable: Settings → Pages → Deploy from branch → main / (root).



Option B: Netlify / Vercel


Works with private repos.



Import the GitHub repo and deploy.



Testing Checklist


Open the live site URL.



Submit a name + email.



Confirm a new row appears in Supabase Table Editor → FanBase.



Submit the same email again to confirm duplicate protection.



Troubleshooting


Nothing saves: verify RLS policy exists and the table name matches  FanBase .



Console error about CORS or network: confirm  SUPABASE_URL  is correct and doesn’t include  /rest/v1 .



Insert blocked: verify you ran the RLS insert policy SQL.



Security Notes


The anon key is designed to be public, but you should still avoid pasting it into public chats.



Rotate keys in Supabase if you believe they were exposed.



For stronger protection against spam, upgrade later to a Supabase Edge Function endpoint with validation/rate limiting.


