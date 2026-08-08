<!doctype html>
<html lang="en"><head><script>window["__codeletBootstrap__"]=JSON.parse('{"A":"A","B":"20260807-05-4dc3575","C":{"Abril Fatface":"YACgEZbkUVE,0","Alfa Slab One":"YACgEYS9sJU,0","Anton":"YACgEcYqQ-A,0","Archivo":"YAHO2-t-jNE,0","Arial":"YAGyDvJ_4Ts,0","Bebas Neue":"YACgESME5ew,0","Bricolage Grotesque":"YAFyMcdwzpc,0","Canva Sans":"YAFLd8sKbwc,2","Caveat":"YALBs2ploWQ,0","Comic Sans MS":"YAHO2VMiyZo,0","Cormorant Garamond":"YAFdJhX-538,0","Courier New":"YAGzXiGs0_8,0","DM Sans":"YAD1aU3sLnI,0","DM Serif Display":"YAD1aYG82rc,0","Forum":"YACgEcnnqB4,0","Fraunces":"YAEul-FRQw4,0","Georgia":"YAGzXkO0pEM,0","Helvetica Neue":"YAFcf6CtJfI,0","Impact":"YAFcfnjI7Vk,0","Inter":"YAFdJvSyp_k,3","Iowan Old Style":"YAGNIFa8j9o,0","Jacques Francois":"YAHO2a5g66Q,0","JetBrains Mono":"YAFdJksXcAk,0","Libre Baskerville":"YACgEUFdPdA,0","Manrope":"YAHO2b2feC4,0","Merriweather":"YACgEXvHxxs,0","Montserrat":"YADLjI9qxTA,0","Nunito":"YACgEX8C5Gg,0","Oleo Script":"YACgEQQ14jI,0","Phantom Sans":"YAHO2E8Pb88,0","Playfair Display":"YACgEYmuCJE,0","Poppins":"YAFdJjbTu24,1","Press Start 2P":"YAFyGr-8pmQ,0","Quicksand":"YADWjpfPmdk,0","Raleway":"YACgEVg3xZg,0","Segoe UI":"YAHNdRD1Klw,0","Source Sans 3":"YAG4lO1Mj10,0","Spectral":"YAHO2rVUHIM,0","Times New Roman":"YAGzXW3gftg,0","Times":"YAGzXW3gftg,0","Ubuntu":"YACgERDU--Q,0","Work Sans":"YAGXhLOKv44,0","Yellowtail":"YACgEYG4kG4,0","ui-monospace":"YADlN8CFZ8Q,0","ui-sans-serif":"YACkoN-xg4g,0"}}');</script><script src="/_sdk/7949ff62d67710d5.telemetry_sdk.js" integrity="sha512-KIvXA82Di44YY/RH9/63A9MuTuavYgDFG8PfErJn7Wli4K0LAOk+coo/aPXk3+ZNL96nHh9VYD4PE+fLes+laQ=="></script>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hood King Community</title>
  <script src="https://cdn.tailwindcss.com/3.4.17"></script>
  <script src="https://cdn.jsdelivr.net/npm/lucide@0.263.0/dist/umd/lucide.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2.46.2/dist/umd/supabase.js"></script>
  <script src="/_sdk/04cc6185e046f597.resizing_sdk.js" type="text/javascript" integrity="sha512-CiE/G92aQF0nxneFg1kdOvXih8sQ1Z2a2QI3+r/WvzJwQqH6+IyB3iL07OkJmpm3ABAaf07+FnqWny98f5sR6w=="></script>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&amp;family=Raleway:wght@400;500;600;700;800&amp;display=swap" rel="stylesheet">
  <style>
    :root {
      --red: #dc143c;
      --ink: #000000;
      --panel: #0a0a0a;
      --muted: #b7b7b7;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: "Raleway", sans-serif;
      background: #000;
    }

    .app-shell {
      width: 100%;
      min-height: calc(100 * min(var(--vh, 1vh), 1vh));
      position: relative;
      overflow: hidden;
      background: #000;
    }

    .app-shell::before {
      content: "";
      position: absolute;
      inset: 0;
      opacity: .08;
      pointer-events: none;
      background-image:
        linear-gradient(rgba(255, 255, 255, .15) 1px, transparent 1px),
        linear-gradient(90deg, rgba(255, 255, 255, .15) 1px, transparent 1px);
      background-size: 42px 42px;
      mask-image: linear-gradient(to bottom, black, transparent 72%);
    }

    .gold-line {
      height: 1px;
      background: linear-gradient(90deg, transparent, #ffffff, transparent);
    }

    .hero-image-wrap::after {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(90deg, rgba(0,0,0,.97) 2%, rgba(0,0,0,.62) 50%, rgba(0,0,0,.14) 100%);
    }

    .hero-image-wrap img {
      filter: saturate(.95) contrast(1.15) brightness(.86);
    }

    .benefit-card {
      transition: transform .28s ease, border-color .28s ease, background .28s ease;
    }

    .benefit-card:hover {
      transform: translateY(-4px);
      border-color: rgba(220, 20, 60, .7);
      background: #141414;
    }

    .reveal { animation: reveal .7s both cubic-bezier(.2,.8,.2,1); }
    .reveal-2 { animation: reveal .7s .13s both cubic-bezier(.2,.8,.2,1); }
    .reveal-3 { animation: reveal .7s .24s both cubic-bezier(.2,.8,.2,1); }

    @keyframes reveal {
      from { opacity: 0; transform: translateY(18px); }
      to { opacity: 1; transform: translateY(0); }
    }

    input:focus,
    textarea:focus {
      outline: 2px solid var(--red);
      outline-offset: 2px;
    }

    button:focus-visible,
    a:focus-visible {
      outline: 2px solid #ff4466;
      outline-offset: 3px;
    }

    .form-field {
      width: 100%;
      border: 1px solid rgba(255,255,255,.3);
      background: #0f0f0f;
      color: #fff;
      font-family: "DM Sans", sans-serif;
      transition: border-color .2s ease, background .2s ease;
    }

    .form-field:hover {
      border-color: rgba(255,255,255,.55);
      background: #151515;
    }

    .form-status {
      min-height: 22px;
      margin: 0;
      font-family: "DM Sans", sans-serif;
    }

    .status-error { color: #ff8a9f; }
    .status-loading { color: #d6d6d6; }
  </style>
  <script src="/_sdk/0e8d3a91e1c6f495.data_sdk.js" type="text/javascript" integrity="sha512-c00oDoGjsMgluCLLEyVl3suwEkgjOGGplVFbsilUoBg4aMKNmsL3mwsc9r0dPn95qiSZyjBousQXgROkAW7p/w=="></script>
 </head>
 <body data-template-id="__page-root" style="background: rgb(0, 0, 0);">
  <div class="app-shell text-white">
   <header class="relative z-10 w-full px-5 pt-5 sm:px-8 lg:px-12">
    <nav class="mx-auto flex max-w-6xl items-center justify-between border-b border-white/10 pb-4" aria-label="Main navigation"><a href="#join" class="flex items-center gap-2.5 no-underline"> <span class="flex h-9 w-9 items-center justify-center border border-white/40 text-white" aria-hidden="true"> <i data-lucide="crown" style="width:18px;height:18px"></i> </span> <span data-template-id="nav-brand" class="canva-text text-sm font-extrabold uppercase tracking-[0.18em]" style="color: rgb(255, 255, 255); font-weight: 800; font-style: normal; font-size: 16px;">Hood King</span> </a> <a data-template-id="nav-join-link" class="canva-link text-xs font-bold uppercase tracking-[0.16em] no-underline transition hover:brightness-125" href="#join" style="color: rgb(220, 20, 60); font-weight: 700; font-style: normal; font-size: 16px;">Claim your place</a>
    </nav>
   </header>
   <main class="relative z-10 w-full px-5 pb-10 pt-8 sm:px-8 lg:px-12">
    <section class="mx-auto max-w-6xl overflow-hidden border border-white/10 bg-black shadow-2xl shadow-black/40">
     <div class="grid min-h-[560px] lg:grid-cols-[1.05fr_.95fr]">
      <div class="relative order-2 min-h-[310px] lg:order-1 lg:min-h-full">
       <div class="hero-image-wrap absolute inset-0"><img data-template-id="hero-image" class="canva-image h-full w-full object-cover" loading="lazy" src="canva://MAHRcNPLeXc/1" alt="Hood King Entertainment logo featuring a streetwear character and bold white lettering">
       </div>
       <div class="absolute bottom-0 left-0 right-0 z-10 p-6 sm:p-8 lg:p-10">
        <div class="gold-line mb-4 w-20"></div>
        <p data-template-id="hero-photo-caption" class="canva-text max-w-xs text-xs font-medium uppercase tracking-[0.16em] text-white/70" style="color: rgb(255, 255, 255); font-weight: 600; font-style: normal; font-size: 16px;">Built for the ones setting the pace.</p>
       </div>
      </div>
      <div id="join" class="order-1 flex flex-col justify-center p-7 sm:p-10 lg:order-2 lg:p-14">
       <div class="reveal">
        <p data-template-id="hero-eyebrow" class="canva-text mb-5 text-xs font-bold uppercase tracking-[0.23em]" style="color: rgb(220, 20, 60); font-weight: 700; font-style: normal; font-size: 16px;">The inner circle</p>
        <h1 data-template-id="hero-title" class="canva-text max-w-xl font-extrabold uppercase leading-[.93] tracking-[-0.045em]" style="color: rgb(255, 255, 255); font-weight: 800; font-style: normal; font-size: 52px; line-height: 0.93;">Hood King Community</h1>
        <div class="gold-line my-7 w-24"></div>
       </div>
       <p data-template-id="hero-description" class="canva-text reveal-2 max-w-lg leading-relaxed text-white/70" style="color: rgb(224, 224, 224); font-weight: 400; font-style: normal; font-size: 18px; line-height: 1.55;">Your direct line to rare drops, real stories, and the people moving culture forward. Join the list. Stay ahead of the noise.</p>
       <p data-template-id="vip-note" class="canva-text reveal-2 mt-5 text-xs font-semibold uppercase tracking-[0.12em]" style="color: rgb(220, 20, 60); font-weight: 700; font-style: normal; font-size: 16px;">Private updates · Zero filler · All access</p>
       <div class="reveal-3 mt-8">
        <form id="signup-form" class="space-y-4" novalidate="">
         <div><label data-template-id="name-label" class="canva-text mb-2 block text-xs font-bold uppercase tracking-[0.15em]" for="name" style="color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 16px;">Your name</label> <input id="name" data-template-id="name-input" class="canva-input form-field px-4 py-4 text-sm placeholder:text-white/40" type="text" autocomplete="name" required="" placeholder="First and last name" style="background: rgb(15, 15, 15); color: rgb(255, 255, 255); font-weight: 400; font-style: normal; font-size: 16px;">
         </div>
         <div><label data-template-id="email-label" class="canva-text mb-2 block text-xs font-bold uppercase tracking-[0.15em]" for="email" style="color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 16px;">Your email address</label> <input id="email" data-template-id="email-input" class="canva-input form-field px-4 py-4 text-sm placeholder:text-white/40" type="email" autocomplete="email" required="" placeholder="name@email.com" style="background: rgb(15, 15, 15); color: rgb(255, 255, 255); font-weight: 400; font-style: normal; font-size: 16px;">
         </div>
         <div><label data-template-id="interests-label" class="canva-text mb-2 block text-xs font-bold uppercase tracking-[0.15em]" for="interests" style="color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 16px;">What are you into? (optional)</label> <input id="interests" data-template-id="interests-input" class="canva-input form-field px-4 py-4 text-sm placeholder:text-white/40" type="text" autocomplete="off" placeholder="Drops, events, music, culture..." style="background: rgb(15, 15, 15); color: rgb(255, 255, 255); font-weight: 400; font-style: normal; font-size: 16px;">
         </div><button id="join-button" data-template-id="join-button" class="canva-button inline-flex min-h-[54px] w-full items-center justify-center gap-2 px-6 py-3 text-sm font-extrabold uppercase tracking-[0.12em] transition hover:brightness-110 disabled:cursor-wait disabled:opacity-60" type="submit" style="background: rgb(220, 20, 60); color: rgb(0, 0, 0); font-weight: 800;"> <span id="join-default-label" data-template-id="join-button-label" class="canva-text" style="color: rgb(0, 0, 0); font-weight: 800; font-style: normal; font-size: 16px;">Join now</span> <span id="join-loading-label" data-template-id="join-loading-label" class="canva-text hidden" style="color: rgb(0, 0, 0); font-weight: 800; font-style: normal; font-size: 16px;">Saving</span> <i id="join-icon" data-lucide="arrow-up-right" style="width:17px;height:17px"></i> </button>
         <p id="form-message" class="form-status" aria-live="polite"></p>
        </form>
        <section id="signup-success" class="hidden border border-white/30 bg-white/5 p-5" aria-live="polite" aria-labelledby="success-heading">
         <div class="flex gap-3"><i data-lucide="badge-check" class="mt-0.5 shrink-0 text-white" style="width:22px;height:22px" aria-hidden="true"></i>
          <div>
           <h2 id="success-heading" data-template-id="success-title" class="canva-text font-bold" style="color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 24px;">You're on the list.</h2>
           <p data-template-id="success-copy" class="canva-text mt-1 leading-relaxed text-white/70" style="color: rgb(224, 224, 224); font-weight: 400; font-style: normal; font-size: 16px; line-height: 1.5;">Welcome to the inner circle. Keep an eye on your inbox for your first Hood King update.</p>
          </div>
         </div>
        </section>
       </div>
      </div>
     </div>
    </section>
    <section class="mx-auto max-w-6xl pt-12 sm:pt-16" aria-labelledby="benefits-heading">
     <div class="mb-6 flex items-end justify-between gap-5">
      <div>
       <p data-template-id="benefits-eyebrow" class="canva-text text-xs font-bold uppercase tracking-[0.2em]" style="color: rgb(220, 20, 60); font-weight: 700; font-style: normal; font-size: 16px;">Membership has its privileges</p>
       <h2 id="benefits-heading" data-template-id="benefits-title" class="canva-text mt-2 font-bold uppercase tracking-[-0.025em]" style="color: rgb(255, 255, 255); font-weight: 800; font-style: normal; font-size: 24px;">What hits your inbox</h2>
      </div><i data-lucide="sparkles" class="hidden text-white sm:block" style="width:26px;height:26px" aria-hidden="true"></i>
     </div>
     <div class="grid gap-3 sm:grid-cols-2 lg:grid-cols-4">
      <article data-template-id="benefit-card-1" class="canva-card benefit-card border border-white/20 p-5" style="background: rgb(10, 10, 10);"><i data-lucide="gem" class="mb-6 text-white" style="width:22px;height:22px" aria-hidden="true"></i>
       <h3 data-template-id="benefit-title-1" class="canva-text font-bold uppercase tracking-[0.04em]" style="color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 19px;">Exclusive drops</h3>
       <p data-template-id="benefit-copy-1" class="canva-text mt-2 text-sm leading-relaxed text-white/60" style="color: rgb(204, 204, 204); font-weight: 400; font-style: normal; font-size: 16px;">First word on limited releases, special offers, and rare finds.</p>
      </article>
      <article data-template-id="benefit-card-2" class="canva-card benefit-card border border-white/20 p-5" style="background: rgb(10, 10, 10);"><i data-lucide="eye" class="mb-6 text-white" style="width:22px;height:22px" aria-hidden="true"></i>
       <h3 data-template-id="benefit-title-2" class="canva-text font-bold uppercase tracking-[0.04em]" style="color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 19px;">Behind the scenes</h3>
       <p data-template-id="benefit-copy-2" class="canva-text mt-2 text-sm leading-relaxed text-white/60" style="color: rgb(204, 204, 204); font-weight: 400; font-style: normal; font-size: 16px;">The untold process, people, and energy behind every move.</p>
      </article>
      <article data-template-id="benefit-card-3" class="canva-card benefit-card border border-white/20 p-5" style="background: rgb(10, 10, 10);"><i data-lucide="zap" class="mb-6 text-white" style="width:22px;height:22px" aria-hidden="true"></i>
       <h3 data-template-id="benefit-title-3" class="canva-text font-bold uppercase tracking-[0.04em]" style="color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 19px;">Early access</h3>
       <p data-template-id="benefit-copy-3" class="canva-text mt-2 text-sm leading-relaxed text-white/60" style="color: rgb(204, 204, 204); font-weight: 400; font-style: normal; font-size: 16px;">Get there before the crowd when something worth having lands.</p>
      </article>
      <article data-template-id="benefit-card-4" class="canva-card benefit-card border border-white/20 p-5" style="background: rgb(10, 10, 10);"><i data-lucide="megaphone" class="mb-6 text-white" style="width:22px;height:22px" aria-hidden="true"></i>
       <h3 data-template-id="benefit-title-4" class="canva-text font-bold uppercase tracking-[0.04em]" style="color: rgb(255, 255, 255); font-weight: 700; font-style: normal; font-size: 19px;">Member announcements</h3>
       <p data-template-id="benefit-copy-4" class="canva-text mt-2 text-sm leading-relaxed text-white/60" style="color: rgb(204, 204, 204); font-weight: 400; font-style: normal; font-size: 16px;">Private news and community moments, delivered with intention.</p>
      </article>
     </div>
    </section>
   </main>
   <footer class="relative z-10 w-full px-5 pb-8 sm:px-8 lg:px-12">
    <div class="mx-auto flex max-w-6xl items-center gap-3 border-t border-white/10 pt-5"><span class="h-2 w-2 bg-[#dc143c]" aria-hidden="true"></span>
     <p data-template-id="footer-text" class="canva-text text-xs font-medium uppercase tracking-[0.14em] text-white/50" style="color: rgb(153, 153, 153); font-weight: 600; font-style: normal; font-size: 16px;">Hood King Community — access with intention.</p>
    </div>
   </footer>
  </div>
  <script src="/_sdk/571d88ca352bbccf.editing_sdk.js" integrity="sha512-jpVzCgOJfgU8ETK2cVi9ukdjrZIqXjCspYqy9afx1TyeJ4jZxisBmh2SIlonXgbaxCv9M5yrk3WY4wZKWDC3Ig=="></script>
  <script>
    /*
      Add your project details before publishing.
      Use the public anonymous key from your Supabase project settings.
    */
    const SUPABASE_URL = "https://YOUR_PROJECT.supabase.co";
    const SUPABASE_ANON_KEY = "YOUR_SUPABASE_ANON_KEY";

    document.addEventListener("DOMContentLoaded", () => {
      lucide.createIcons();

      const form = document.getElementById("signup-form");
      const nameInput = document.getElementById("name");
      const emailInput = document.getElementById("email");
      const interestsInput = document.getElementById("interests");
      const button = document.getElementById("join-button");
      const defaultLabel = document.getElementById("join-default-label");
      const loadingLabel = document.getElementById("join-loading-label");
      const joinIcon = document.getElementById("join-icon");
      const message = document.getElementById("form-message");
      const success = document.getElementById("signup-success");

      let supabaseClient = null;

      function showMessage(text, type) {
        message.textContent = text;
        message.className = "form-status " + (type === "error" ? "status-error" : "status-loading");
      }

      function clearMessage() {
        message.textContent = "";
        message.className = "form-status";
      }

      function setLoading(isLoading) {
        button.disabled = isLoading;
        defaultLabel.classList.toggle("hidden", isLoading);
        loadingLabel.classList.toggle("hidden", !isLoading);
        joinIcon.classList.toggle("hidden", isLoading);
      }

      function hasSupabaseCredentials() {
        return (
          SUPABASE_URL &&
          SUPABASE_ANON_KEY &&
          !SUPABASE_URL.includes("YOUR_PROJECT") &&
          !SUPABASE_ANON_KEY.includes("YOUR_SUPABASE")
        );
      }

      if (hasSupabaseCredentials() && window.supabase) {
        supabaseClient = window.supabase.createClient(SUPABASE_URL, SUPABASE_ANON_KEY);
      }

      form.addEventListener("submit", async (event) => {
        event.preventDefault();
        clearMessage();

        const name = nameInput.value.trim();
        const email = emailInput.value.trim();
        const interests = interestsInput.value.trim();

        if (!name) {
          showMessage("Enter your name to claim your place.", "error");
          nameInput.focus();
          return;
        }

        if (!email || !emailInput.validity.valid) {
          showMessage("Enter a valid email address to join.", "error");
          emailInput.focus();
          return;
        }

        if (!supabaseClient) {
          showMessage("Signups are not connected yet. Add your Supabase project URL and anonymous key to activate the list.", "error");
          return;
        }

        setLoading(true);
        showMessage("Saving your place in the inner circle...", "loading");

        const { error } = await supabaseClient
          .from("fans")
          .insert({
            name: name,
            email: email,
            interests: interests || null
          });

        if (error) {
          showMessage("Your spot was not saved. Please check your details and try again.", "error");
          setLoading(false);
          return;
        }

        form.classList.add("hidden");
        success.classList.remove("hidden");
      });
    });
  </script>
 
</body></html>
