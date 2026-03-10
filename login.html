<!DOCTYPE html>
<html lang="nl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>AutoPanel — Inloggen</title>
<link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700;800&family=DM+Sans:wght@400;500&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/@supabase/supabase-js@2"></script>
<style>
*,*::before,*::after{margin:0;padding:0;box-sizing:border-box}
:root{--bg:#0a0c12;--surface:#11141d;--surface2:#181c28;--border:#232840;--text:#eef0f6;--text2:#7a82a0;--text3:#404868;--accent:#e8f03c;--red:#e83c6a;--green:#3ce890}
body{font-family:'DM Sans',sans-serif;background:var(--bg);color:var(--text);min-height:100vh;display:flex;align-items:center;justify-content:center;padding:20px;position:relative;overflow:hidden}
body::before{content:'';position:fixed;inset:0;background-image:linear-gradient(var(--border) 1px,transparent 1px),linear-gradient(90deg,var(--border) 1px,transparent 1px);background-size:48px 48px;opacity:.3;pointer-events:none}
body::after{content:'';position:fixed;top:-20%;left:50%;transform:translateX(-50%);width:600px;height:400px;background:radial-gradient(ellipse,rgba(232,240,60,.06) 0%,transparent 70%);pointer-events:none}
.card{width:100%;max-width:420px;background:var(--surface);border:1px solid var(--border);box-shadow:0 24px 64px rgba(0,0,0,.6);position:relative;z-index:1;animation:up .4s cubic-bezier(.4,0,.2,1)}
@keyframes up{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}}
.card-top{padding:32px 32px 0;text-align:center}
.logo{display:inline-flex;align-items:center;gap:10px;margin-bottom:28px}
.logo-mark{width:36px;height:36px;background:var(--accent);display:flex;align-items:center;justify-content:center;font-family:'Outfit',sans-serif;font-weight:800;font-size:13px;color:#000;letter-spacing:-.5px}
.logo-name{font-family:'Outfit',sans-serif;font-weight:700;font-size:17px}
.tabs{display:flex;border-bottom:1px solid var(--border);margin:0 -1px}
.tab{flex:1;padding:13px 0;font-size:13px;font-weight:500;color:var(--text2);cursor:pointer;border-bottom:2px solid transparent;margin-bottom:-1px;transition:all .2s;text-align:center;user-select:none}
.tab:hover{color:var(--text)}
.tab.active{color:var(--accent);border-bottom-color:var(--accent)}
.card-body{padding:28px 32px 32px}
.form{display:none}.form.active{display:block;animation:fi .25s}
@keyframes fi{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:translateY(0)}}
.form-title{font-family:'Outfit',sans-serif;font-weight:700;font-size:20px;margin-bottom:4px;letter-spacing:-.3px}
.form-sub{font-size:13px;color:var(--text2);margin-bottom:22px;line-height:1.5}
.field{margin-bottom:14px}
.field-row{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.label{display:block;font-size:11.5px;font-weight:500;color:var(--text2);margin-bottom:5px}
.input{width:100%;background:var(--surface2);border:1px solid var(--border);padding:10px 13px;color:var(--text);font-family:'DM Sans',sans-serif;font-size:14px;outline:none;border-radius:2px;transition:border-color .15s}
.input:focus{border-color:var(--accent)}
.input::placeholder{color:var(--text3)}
.input.err{border-color:var(--red)}
select.input{cursor:pointer;-webkit-appearance:none;appearance:none}
.field-pw{position:relative}
.field-pw .input{padding-right:42px}
.pw-eye{position:absolute;right:11px;top:50%;transform:translateY(-50%);background:none;border:none;color:var(--text3);cursor:pointer;font-size:14px;padding:4px;transition:color .15s}
.pw-eye:hover{color:var(--text2)}
.hint{font-size:11px;color:var(--text3);margin-top:4px}
.err-msg{font-size:11px;color:var(--red);margin-top:4px;display:none}
.err-msg.show{display:block}
.alert{padding:11px 13px;font-size:13px;line-height:1.5;margin-bottom:14px;border-radius:2px;display:none}
.alert.show{display:block}
.alert-err{background:rgba(232,60,106,.1);border:1px solid rgba(232,60,106,.25);color:var(--red)}
.alert-warn{background:rgba(232,240,60,.08);border:1px solid rgba(232,240,60,.2);color:var(--accent)}
.btn{width:100%;padding:12px;background:var(--accent);color:#000;font-family:'Outfit',sans-serif;font-weight:700;font-size:14px;border:none;cursor:pointer;border-radius:2px;margin-top:6px;transition:background .15s;letter-spacing:.2px}
.btn:hover{background:#d4da2e}
.btn:disabled{background:var(--border);color:var(--text3);cursor:not-allowed}
.pending-box{display:none;text-align:center;padding:16px 0 8px}
.pending-box.show{display:block;animation:fi .3s}
.pending-icon{font-size:38px;margin-bottom:10px}
.pending-title{font-family:'Outfit',sans-serif;font-weight:700;font-size:18px;margin-bottom:7px}
.pending-text{font-size:13px;color:var(--text2);line-height:1.6}
.card-foot{padding:13px 32px 18px;border-top:1px solid var(--border);text-align:center;font-size:12px;color:var(--text3)}
.card-foot a{color:var(--text2);text-decoration:none}
.card-foot a:hover{color:var(--accent)}
@media(max-width:480px){.card-top,.card-body,.card-foot{padding-left:18px;padding-right:18px}.field-row{grid-template-columns:1fr}}
</style>
</head>
<body>
<div class="card">
  <div class="card-top">
    <div class="logo"><div class="logo-mark">AP</div><span class="logo-name">AutoPanel</span></div>
    <div class="tabs">
      <div class="tab active" onclick="switchTab('login')">Inloggen</div>
      <div class="tab" onclick="switchTab('register')">Aanmelden</div>
    </div>
  </div>
  <div class="card-body">

    <!-- LOGIN -->
    <div class="form active" id="form-login">
      <div class="form-title">Welkom terug</div>
      <div class="form-sub">Log in op je AutoPanel account</div>
      <div class="alert alert-err" id="login-err"></div>
      <div class="alert alert-warn" id="login-pending">⏳ Je account wacht nog op goedkeuring. Je ontvangt een e-mail zodra je toegang hebt.</div>
      <div class="field">
        <label class="label">E-mailadres</label>
        <input type="email" class="input" id="l-email" placeholder="jouw@bedrijf.nl" autocomplete="email">
      </div>
      <div class="field">
        <label class="label">Wachtwoord</label>
        <div class="field-pw">
          <input type="password" class="input" id="l-pwd" placeholder="••••••••" autocomplete="current-password">
          <button class="pw-eye" onclick="togglePw('l-pwd',this)" tabindex="-1">👁</button>
        </div>
      </div>
      <div style="display:flex;justify-content:flex-end;margin-bottom:18px">
        <a href="#" style="font-size:12px;color:var(--text2);text-decoration:none" onclick="forgotPassword(event)">Wachtwoord vergeten?</a>
      </div>
      <button class="btn" id="login-btn" onclick="doLogin()">Inloggen</button>
    </div>

    <!-- REGISTER -->
    <div class="form" id="form-register">
      <div class="form-title">Account aanvragen</div>
      <div class="form-sub">Na goedkeuring ontvang je toegang via e-mail</div>
      <div class="alert alert-err" id="reg-err"></div>
      <div class="pending-box" id="pending-box">
        <div class="pending-icon">⏳</div>
        <div class="pending-title">Aanvraag ingediend</div>
        <div class="pending-text">Je aanvraag is ontvangen.<br>Je hoort van ons op <strong id="pending-email-shown"></strong>.</div>
      </div>
      <div id="reg-fields">
        <div class="field field-row">
          <div class="field">
            <label class="label">Voornaam</label>
            <input type="text" class="input" id="r-first" placeholder="Jan" autocomplete="given-name">
            <div class="err-msg" id="e-first">Vul je voornaam in</div>
          </div>
          <div class="field">
            <label class="label">Achternaam</label>
            <input type="text" class="input" id="r-last" placeholder="de Vries" autocomplete="family-name">
            <div class="err-msg" id="e-last">Vul je achternaam in</div>
          </div>
        </div>
        <div class="field">
          <label class="label">Bedrijfsnaam</label>
          <input type="text" class="input" id="r-company" placeholder="Autobedrijf De Vries" autocomplete="organization">
          <div class="err-msg" id="e-company">Vul je bedrijfsnaam in</div>
        </div>
        <div class="field">
          <label class="label">Type bedrijf</label>
          <select class="input" id="r-type">
            <option value="">Selecteer type…</option>
            <option value="dealer">Autodealer</option>
            <option value="garage">Garagebedrijf</option>
            <option value="inkoper">Inkoper / handelaar</option>
            <option value="veiling">Veilingbedrijf</option>
            <option value="ander">Anders</option>
          </select>
          <div class="err-msg" id="e-type">Selecteer een type</div>
        </div>
        <div class="field">
          <label class="label">E-mailadres</label>
          <input type="email" class="input" id="r-email" placeholder="jouw@bedrijf.nl" autocomplete="email">
          <div class="err-msg" id="e-email">Vul een geldig e-mailadres in</div>
        </div>
        <div class="field">
          <label class="label">Telefoonnummer <span style="color:var(--text3);font-size:11px">(optioneel)</span></label>
          <input type="tel" class="input" id="r-phone" placeholder="06 12345678" autocomplete="tel">
        </div>
        <div class="field">
          <label class="label">Wachtwoord</label>
          <div class="field-pw">
            <input type="password" class="input" id="r-pwd" placeholder="Minimaal 8 tekens" autocomplete="new-password">
            <button class="pw-eye" onclick="togglePw('r-pwd',this)" tabindex="-1">👁</button>
          </div>
          <div class="err-msg" id="e-pwd">Minimaal 8 tekens</div>
        </div>
        <div class="field">
          <label class="label">Wachtwoord bevestigen</label>
          <div class="field-pw">
            <input type="password" class="input" id="r-pwd2" placeholder="Herhaal wachtwoord" autocomplete="new-password">
            <button class="pw-eye" onclick="togglePw('r-pwd2',this)" tabindex="-1">👁</button>
          </div>
          <div class="err-msg" id="e-pwd2">Wachtwoorden komen niet overeen</div>
        </div>
        <button class="btn" id="reg-btn" onclick="doRegister()">Aanvraag indienen</button>
      </div>
    </div>

  </div>
  <div class="card-foot">autopanel.nl &nbsp;·&nbsp; <a href="mailto:info@autopanel.nl">Contact</a> &nbsp;·&nbsp; <a href="#">Privacy</a></div>
</div>

<script>
// ─── Supabase init ───────────────────────────────────────────
const SUPABASE_URL      = 'https://jouwprojectid.supabase.co'; // ← aanpassen
const SUPABASE_ANON_KEY = 'jouw-anon-key';                     // ← aanpassen
const { createClient } = supabase;
const sb = createClient(SUPABASE_URL, SUPABASE_ANON_KEY);

// Controleer of al ingelogd
(async () => {
  const { data: { session } } = await sb.auth.getSession();
  if (session) {
    const { data: profile } = await sb.from('profiles').select('status,role').eq('id', session.user.id).single();
    if (profile?.status === 'approved') {
      window.location.href = profile.role === 'admin' ? '/admin/' : '/app.html';
    }
  }
  // Check URL param voor pending redirect
  if (new URLSearchParams(location.search).get('status') === 'pending') {
    document.getElementById('login-pending').classList.add('show');
  }
})();

// ─── Tab switch ───────────────────────────────────────────────
function switchTab(t) {
  ['login','register'].forEach(x => {
    document.getElementById('form-'+x).classList.toggle('active', x===t);
    document.querySelectorAll('.tab')[x==='login'?0:1].classList.toggle('active', x===t);
  });
}

// ─── Helpers ─────────────────────────────────────────────────
function togglePw(id, btn) {
  const i = document.getElementById(id);
  const show = i.type === 'password';
  i.type = show ? 'text' : 'password';
  btn.textContent = show ? '🙈' : '👁';
}
function setLoading(btnId, loading, label='Inloggen') {
  const b = document.getElementById(btnId);
  b.disabled = loading;
  b.textContent = loading ? 'Bezig…' : label;
}
function clearErrs() {
  document.querySelectorAll('.err-msg').forEach(e => e.classList.remove('show'));
  document.querySelectorAll('.input').forEach(e => e.classList.remove('err'));
}
function showErr(fieldId, msgId) {
  document.getElementById(fieldId)?.classList.add('err');
  document.getElementById(msgId)?.classList.add('show');
}

// ─── Login ────────────────────────────────────────────────────
async function doLogin() {
  clearErrs();
  document.getElementById('login-err').classList.remove('show');
  document.getElementById('login-pending').classList.remove('show');

  const email = document.getElementById('l-email').value.trim();
  const pwd   = document.getElementById('l-pwd').value;
  if (!email || !pwd) {
    document.getElementById('login-err').textContent = 'Vul je e-mailadres en wachtwoord in.';
    document.getElementById('login-err').classList.add('show');
    return;
  }

  setLoading('login-btn', true);
  try {
    const { data, error } = await sb.auth.signInWithPassword({ email, password: pwd });
    if (error) throw error;

    const { data: profile } = await sb.from('profiles').select('status,role').eq('id', data.user.id).single();

    if (profile?.status === 'pending') {
      await sb.auth.signOut();
      document.getElementById('login-pending').classList.add('show');
      return;
    }
    if (profile?.status === 'revoked') {
      await sb.auth.signOut();
      document.getElementById('login-err').textContent = 'Je toegang is ingetrokken. Neem contact op via info@autopanel.nl.';
      document.getElementById('login-err').classList.add('show');
      return;
    }

    window.location.href = profile?.role === 'admin' ? '/admin/' : '/app.html';

  } catch(e) {
    document.getElementById('login-err').textContent = 'E-mailadres of wachtwoord is onjuist.';
    document.getElementById('login-err').classList.add('show');
  } finally {
    setLoading('login-btn', false, 'Inloggen');
  }
}

// ─── Register ─────────────────────────────────────────────────
async function doRegister() {
  clearErrs();
  document.getElementById('reg-err').classList.remove('show');

  const first   = document.getElementById('r-first').value.trim();
  const last    = document.getElementById('r-last').value.trim();
  const company = document.getElementById('r-company').value.trim();
  const type    = document.getElementById('r-type').value;
  const email   = document.getElementById('r-email').value.trim();
  const phone   = document.getElementById('r-phone').value.trim();
  const pwd     = document.getElementById('r-pwd').value;
  const pwd2    = document.getElementById('r-pwd2').value;

  let valid = true;
  if (!first)              { showErr('r-first','e-first');   valid=false; }
  if (!last)               { showErr('r-last','e-last');     valid=false; }
  if (!company)            { showErr('r-company','e-company');valid=false; }
  if (!type)               { showErr('r-type','e-type');     valid=false; }
  if (!email||!email.includes('@')) { showErr('r-email','e-email'); valid=false; }
  if (pwd.length < 8)      { showErr('r-pwd','e-pwd');       valid=false; }
  if (pwd !== pwd2)        { showErr('r-pwd2','e-pwd2');     valid=false; }
  if (!valid) return;

  setLoading('reg-btn', true, 'Aanvraag indienen');
  try {
    const { error } = await sb.auth.signUp({
      email, password: pwd,
      options: {
        data: { first_name: first, last_name: last, company, company_type: type, phone }
      }
    });
    if (error) {
      if (error.message.includes('already registered')) {
        document.getElementById('reg-err').textContent = 'Dit e-mailadres is al geregistreerd.';
        document.getElementById('reg-err').classList.add('show');
        return;
      }
      throw error;
    }
    // Toon pending bevestiging
    document.getElementById('pending-email-shown').textContent = email;
    document.getElementById('reg-fields').style.display = 'none';
    document.getElementById('pending-box').classList.add('show');

  } catch(e) {
    document.getElementById('reg-err').textContent = 'Er ging iets mis. Probeer het opnieuw.';
    document.getElementById('reg-err').classList.add('show');
  } finally {
    setLoading('reg-btn', false, 'Aanvraag indienen');
  }
}

// ─── Wachtwoord vergeten ──────────────────────────────────────
async function forgotPassword(e) {
  e.preventDefault();
  const email = document.getElementById('l-email').value.trim();
  if (!email) {
    document.getElementById('login-err').textContent = 'Vul eerst je e-mailadres in hierboven.';
    document.getElementById('login-err').classList.add('show');
    return;
  }
  await sb.auth.resetPasswordForEmail(email, { redirectTo: 'https://autopanel.nl/reset-password' });
  document.getElementById('login-err').style.cssText='display:block;background:rgba(60,232,144,.1);border:1px solid rgba(60,232,144,.25);color:var(--green)';
  document.getElementById('login-err').textContent = '✓ Controleer je e-mail voor een resetlink.';
  document.getElementById('login-err').classList.add('show');
}

// Enter key
document.addEventListener('keydown', e => {
  if (e.key !== 'Enter') return;
  if (document.getElementById('form-login').classList.contains('active')) doLogin();
  else doRegister();
});
</script>
</body>
</html>
