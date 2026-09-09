<!DOCTYPE html>
<html>
<head>
<base target="_top">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&family=Inter:wght@400;500;600&family=IBM+Plex+Mono:wght@500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --ink:      #12212E;
    --paper:    #EDF1F4;
    --card:     #FFFFFF;
    --line:     #C9D2DA;
    --muted:    #5D6E7C;
    --prefer:   #0F6B52;
    --prefer-bg:#DCEDE6;
    --block:    #9C3535;
    --block-bg: #F4DEDE;

    /* Day types. Kept pale on purpose — these are the background, not the
       message. Saturday stays plain so the tinted days read as the exceptions. */
    --sat-bg:   #FFFFFF;
    --sun-bg:   #E7EEF5;
    --sun-ink:  #3A5A76;
    --ph-bg:    #FBF1DC;
    --ph-line:  #E2CB99;
    --ph-ink:   #8A5A12;
  }

  * { box-sizing: border-box; }

  body {
    margin: 0;
    padding: 0 0 108px;
    background: var(--paper);
    color: var(--ink);
    font-family: 'Inter', system-ui, sans-serif;
    font-size: 15px;
    line-height: 1.5;
    -webkit-font-smoothing: antialiased;
  }

  .wrap { max-width: 620px; margin: 0 auto; padding: 0 16px; }

  /* ---------- masthead ---------- */
  header {
    background: var(--ink);
    color: #fff;
    padding: 22px 0 20px;
    margin-bottom: 20px;
  }
  .eyebrow {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #8FA6B6;
    margin-bottom: 6px;
  }
  h1 {
    font-family: 'Space Grotesk', sans-serif;
    font-weight: 700;
    font-size: 26px;
    line-height: 1.15;
    margin: 0 0 10px;
    letter-spacing: -0.01em;
  }
  .meta {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 12px;
    color: #B4C6D2;
  }
  .meta strong { color: #fff; font-weight: 600; }

  /* ---------- blocks ---------- */
  .months {
    display: flex;
    gap: 0;
    margin: -4px 0 16px;
  }
  .months button {
    flex: 1;
    font-family: 'Inter', sans-serif;
    font-size: 13px;
    font-weight: 500;
    color: var(--muted);
    background: var(--card);
    border: 1px solid var(--line);
    padding: 10px 6px;
    margin-left: -1px;
    cursor: pointer;
    line-height: 1.3;
  }
  .months button:first-child { margin-left: 0; border-radius: 3px 0 0 3px; }
  .months button:last-child { border-radius: 0 3px 3px 0; }
  .months button:focus-visible { outline: 2px solid var(--ink); outline-offset: 1px; z-index: 2; }
  .months button[aria-selected="true"] {
    background: var(--ink);
    border-color: var(--ink);
    color: #fff;
    font-weight: 600;
  }
  .months .tick { color: var(--prefer); font-weight: 700; }
  .months button[aria-selected="true"] .tick { color: #7FD3B4; }
  .months .sub {
    display: block;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 9px;
    letter-spacing: 0.06em;
    text-transform: uppercase;
    opacity: 0.75;
    margin-top: 2px;
  }

  .early-note {
    background: #FFF8E8;
    border: 1px solid var(--ph-line);
    border-radius: 3px;
    padding: 10px 12px;
    margin-bottom: 16px;
    font-size: 13px;
    color: #6B4A12;
  }

  .block {
    background: var(--card);
    border: 1px solid var(--line);
    border-radius: 4px;
    padding: 16px;
    margin-bottom: 16px;
  }
  label.field {
    display: block;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--muted);
    margin-bottom: 8px;
  }
  select, input[type=number], textarea {
    width: 100%;
    font-family: 'Inter', sans-serif;
    font-size: 16px;
    color: var(--ink);
    background: #fff;
    border: 1px solid var(--line);
    border-radius: 3px;
    padding: 11px 12px;
  }
  textarea { resize: vertical; min-height: 68px; }
  .hint { font-size: 13px; color: var(--muted); margin-top: 8px; }

  /* ---------- date rows ---------- */
  .section-title {
    font-family: 'Space Grotesk', sans-serif;
    font-weight: 700;
    font-size: 17px;
    margin: 26px 0 4px;
  }
  .section-note { font-size: 13px; color: var(--muted); margin-bottom: 12px; }

  /* Two independent channels: the fill says what kind of day it is, the left
     stripe says what you chose. Overloading one channel meant that marking a
     public holiday as preferred erased the fact that it was a holiday. */
  .day {
    display: flex;
    align-items: center;
    gap: 14px;
    background: var(--card);
    border: 1px solid var(--line);
    border-left: 5px solid var(--line);
    border-radius: 4px;
    padding: 10px 12px;
    margin-bottom: 8px;
  }
  .day--sat { background: var(--sat-bg); }
  .day--sun { background: var(--sun-bg); border-color: #BFD0DE; }
  .day--sun .dow { color: var(--sun-ink); }
  .day--ph  { background: var(--ph-bg); border-color: var(--ph-line); }
  .day--ph .num, .day--ph .dow { color: var(--ph-ink); }

  .day.is-prefer { border-left-color: var(--prefer); box-shadow: inset 0 0 0 1px var(--prefer); }
  .day.is-block  { border-left-color: var(--block); opacity: 0.55; }

  .legend {
    display: flex;
    flex-wrap: wrap;
    gap: 14px;
    margin-bottom: 12px;
    font-size: 12px;
    color: var(--muted);
  }
  .legend span { display: flex; align-items: center; gap: 6px; }
  .legend i {
    width: 13px; height: 13px; border-radius: 2px;
    border: 1px solid var(--line);
  }
  .legend .sw--sat { background: var(--sat-bg); }
  .legend .sw--sun { background: var(--sun-bg); border-color: #BFD0DE; }
  .legend .sw--ph  { background: var(--ph-bg);  border-color: var(--ph-line); }

  .stamp { min-width: 46px; text-align: center; }
  .stamp .num {
    font-family: 'IBM Plex Mono', monospace;
    font-weight: 600;
    font-size: 26px;
    line-height: 1;
    letter-spacing: -0.02em;
  }
  .stamp .dow {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 10px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--muted);
    margin-top: 3px;
  }
  .ph {
    display: inline-block;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 9px;
    letter-spacing: 0.08em;
    background: var(--ph-ink);
    color: #fff;
    border-radius: 2px;
    padding: 1px 4px;
    margin-top: 4px;
  }

  .seg { display: flex; flex: 1; gap: 0; }
  .seg button {
    flex: 1;
    font-family: 'Inter', sans-serif;
    font-size: 13px;
    font-weight: 500;
    color: var(--muted);
    background: #fff;
    border: 1px solid var(--line);
    padding: 9px 4px;
    cursor: pointer;
    margin-left: -1px;
  }
  .seg button:first-child { margin-left: 0; border-radius: 3px 0 0 3px; }
  .seg button:last-child { border-radius: 0 3px 3px 0; }
  .seg button:focus-visible { outline: 2px solid var(--ink); outline-offset: 1px; z-index: 2; }
  .seg button[aria-pressed="true"] { color: #fff; font-weight: 600; }
  .seg button.v-prefer[aria-pressed="true"] { background: var(--prefer); border-color: var(--prefer); }
  .seg button.v-ok[aria-pressed="true"]     { background: var(--ink);    border-color: var(--ink); }
  .seg button.v-block[aria-pressed="true"]  { background: var(--block);  border-color: var(--block); }

  /* ---------- sticky bar ---------- */
  .bar {
    position: fixed;
    left: 0; right: 0; bottom: 0;
    background: var(--ink);
    color: #fff;
    padding: 12px 16px calc(12px + env(safe-area-inset-bottom));
    display: flex;
    align-items: center;
    gap: 14px;
  }
  .bar .count { flex: 1; }
  .bar .count .n {
    font-family: 'IBM Plex Mono', monospace;
    font-weight: 600;
    font-size: 19px;
  }
  .bar .count .lbl { font-size: 12px; color: #A9BECC; }
  .bar .count .warn { color: #F0B9B9; }
  .bar button {
    font-family: 'Inter', sans-serif;
    font-size: 15px;
    font-weight: 600;
    color: var(--ink);
    background: #fff;
    border: 0;
    border-radius: 3px;
    padding: 12px 22px;
    cursor: pointer;
  }
  .bar button:disabled { opacity: 0.45; cursor: default; }

  .toast {
    position: fixed; left: 16px; right: 16px; bottom: 88px;
    background: var(--prefer); color: #fff;
    border-radius: 3px; padding: 12px 14px; font-size: 14px;
    display: none;
  }
  .toast.err { background: var(--block); }

  .state { padding: 40px 0; text-align: center; color: var(--muted); }
  .hidden { display: none; }

  @media (prefers-reduced-motion: no-preference) {
    .day { transition: background 120ms ease, border-color 120ms ease; }
  }
  @media (max-width: 400px) {
    .day { flex-wrap: wrap; }
    .seg { flex-basis: 100%; }
  }
</style>
</head>
<body>

<header>
  <div class="wrap">
    <div class="eyebrow">Weekend &amp; public holiday rounds</div>
    <h1 id="title">Loading…</h1>
    <div class="meta" id="meta"></div>
  </div>
</header>

<div class="wrap">
  <div id="loading" class="state">Fetching this month's dates…</div>
  <div id="closed" class="state hidden"></div>

  <div id="form" class="hidden">
    <div class="months" id="months" role="tablist"></div>
    <div class="early-note hidden" id="earlyNote"></div>

    <div class="block">
      <label class="field" for="name">Your name</label>
      <select id="name">
        <option value="">Select…</option>
      </select>
      <div class="hint" id="prefillNote"></div>
    </div>

    <div class="section-title">Mark each date</div>
    <div class="section-note">
      Everything starts as <strong>Can round</strong>. Change only what you need to.
      Preferred days are honoured where the numbers allow; they are not guaranteed.
    </div>
    <div class="legend" id="legend"></div>
    <div id="days"></div>

    <div class="block" style="margin-top:20px">
      <label class="field" for="maxDays">Cap my days this month (optional)</label>
      <input type="number" id="maxDays" min="1" max="31" placeholder="Leave blank for no cap">
    </div>

    <div class="block">
      <label class="field" for="notes">Anything the planner should know</label>
      <textarea id="notes" maxlength="500" placeholder="e.g. away 12–14 Sep, happy to take extra the following weekend"></textarea>
    </div>
  </div>
</div>

<div class="bar hidden" id="bar">
  <div class="count">
    <span class="n" id="availNum">—</span>
    <span class="lbl" id="availLbl"></span>
  </div>
  <button id="save" disabled>Save</button>
</div>

<div class="toast" id="toast"></div>

<script>
  /* ------------------------------------------------------------------
     PASTE YOUR WEB APP URL HERE. Deploy → Manage deployments → copy the
     URL ending in /exec. It does not change when you redeploy.
     ------------------------------------------------------------------ */
  var API_URL = 'https://script.google.com/macros/s/AKfycbziFNlonOclvsvPLQx3a6VPfbV0UOD6s9W3i5Jm1mw_84bvnkiDIKlM462DtWmiT1nuzA/exec';

  /* We talk to Apps Script over fetch rather than google.script.run.
     google.script.run resolves against the browser's default Google account,
     so anyone signed into two accounts gets errors or someone else's session.
     Plain HTTP has no account to resolve. */

  function apiGet(action, params) {
    var q = '?action=' + encodeURIComponent(action);
    Object.keys(params || {}).forEach(function (k) {
      q += '&' + k + '=' + encodeURIComponent(params[k]);
    });
    return fetch(API_URL + q)
      .then(function (r) { return r.json(); })
      .then(function (d) {
        if (d && d.error) throw new Error(d.error);
        return d;
      });
  }

  function apiPost(payload) {
    return fetch(API_URL, {
      method: 'POST',
      // text/plain, not application/json: it keeps the request "simple" so the
      // browser skips the CORS preflight, which Apps Script cannot answer.
      headers: { 'Content-Type': 'text/plain;charset=utf-8' },
      body: JSON.stringify(payload)
    })
      .then(function (r) { return r.json(); })
      .then(function (d) {
        if (d && d.error) throw new Error(d.error);
        return d;
      });
  }

  var DATA = null;          // full payload: months[] + consultants
  var MONTH = null;         // the month object currently on screen
  // Edits live per month so switching tabs never discards unsaved work.
  var state = {};           // monthKey -> { iso -> 'prefer'|'ok'|'block' }
  var extras = {};          // monthKey -> { maxDays, notes }
  var saved = {};           // monthKey -> savedAt string, or null

  if (API_URL.indexOf('PASTE_') === 0) {
    document.getElementById('loading').textContent =
      'This form has not been configured yet — API_URL is still a placeholder.';
  } else {
    apiGet('form').then(init).catch(fatal);
  }

  function fatal(err) {
    document.getElementById('loading').textContent =
      'Could not load the form. ' + err.message;
  }

  function init(data) {
    DATA = data;
    document.getElementById('loading').classList.add('hidden');

    if (!data.open) {
      var closed = document.getElementById('closed');
      closed.textContent = data.notice ||
        'Submissions are closed. Contact the roster planner if something has changed.';
      closed.classList.remove('hidden');
      return;
    }

    data.months.forEach(function (m) {
      state[m.key] = {};
      m.dates.forEach(function (d) { state[m.key][d.iso] = 'ok'; });
      extras[m.key] = { maxDays: '', notes: '' };
      saved[m.key] = null;
    });

    var select = document.getElementById('name');
    data.consultants.forEach(function (n) {
      var opt = document.createElement('option');
      opt.value = n;
      opt.textContent = n;
      select.appendChild(opt);
    });
    select.addEventListener('change', onNameChange);

    renderMonthTabs();
    selectMonth(data.months[0].key);

    document.getElementById('form').classList.remove('hidden');
    document.getElementById('bar').classList.remove('hidden');
    document.getElementById('save').addEventListener('click', save);
  }

  /* ---------------- months ---------------- */

  function renderMonthTabs() {
    var host = document.getElementById('months');
    host.innerHTML = '';
    if (DATA.months.length < 2) { host.classList.add('hidden'); return; }

    DATA.months.forEach(function (m) {
      var b = document.createElement('button');
      b.type = 'button';
      b.setAttribute('role', 'tab');
      b.id = 'tab-' + m.key;
      b.addEventListener('click', function () { selectMonth(m.key); });
      host.appendChild(b);
    });
    paintMonthTabs();
  }

  function paintMonthTabs() {
    if (DATA.months.length < 2) return;
    var name = document.getElementById('name').value;
    DATA.months.forEach(function (m) {
      var b = document.getElementById('tab-' + m.key);
      b.innerHTML = m.shortLabel +
        (name && saved[m.key] ? ' <span class="tick">&#10003;</span>' : '') +
        '<span class="sub">' + (name
          ? (saved[m.key] ? 'saved' : 'not sent')
          : m.submitted.length + '/' + DATA.consultants.length) + '</span>';
      b.setAttribute('aria-selected', MONTH && m.key === MONTH.key);
    });
  }

  function selectMonth(key) {
    if (MONTH) stashExtras();

    MONTH = null;
    DATA.months.forEach(function (m) { if (m.key === key) MONTH = m; });
    if (!MONTH) return;

    document.getElementById('title').textContent = MONTH.label;

    var meta = MONTH.dates.length + ' rounding days · ' + MONTH.minPerDay + ' needed each day';
    if (MONTH.target) meta += ' · <strong>&#8776;' + MONTH.target + ' each</strong>';
    if (MONTH.deadline) meta += '<br>Closes ' + MONTH.deadline;
    document.getElementById('meta').innerHTML = meta;

    var early = document.getElementById('earlyNote');
    if (MONTH.early) {
      early.textContent = MONTH.label + ' is open early so you can plan ahead. ' +
        'Public holidays are confirmed, but dates may still be adjusted before it goes live.';
      early.classList.remove('hidden');
    } else {
      early.classList.add('hidden');
    }

    document.getElementById('maxDays').value = extras[MONTH.key].maxDays;
    document.getElementById('notes').value = extras[MONTH.key].notes;
    document.getElementById('save').textContent = 'Save ' + MONTH.shortLabel;

    renderDays();
    paintMonthTabs();
    updateCount();
  }

  function stashExtras() {
    extras[MONTH.key] = {
      maxDays: document.getElementById('maxDays').value,
      notes: document.getElementById('notes').value
    };
  }

  /* ---------------- days ---------------- */

  /** Public holiday wins over the weekday it happens to fall on. */
  function dayType(d) {
    if (d.extra) return 'ph';
    if (d.dow === 0) return 'sun';
    return 'sat';
  }

  function renderLegend() {
    var labels = { sat: 'Saturday', sun: 'Sunday', ph: 'Public holiday' };
    var present = {};
    MONTH.dates.forEach(function (d) { present[dayType(d)] = true; });

    var host = document.getElementById('legend');
    host.innerHTML = '';
    ['sat', 'sun', 'ph'].forEach(function (key) {
      if (!present[key]) return;
      var item = document.createElement('span');
      item.innerHTML = '<i class="sw sw--' + key + '"></i>' + labels[key];
      host.appendChild(item);
    });
  }

  function renderDays() {
    renderLegend();
    var host = document.getElementById('days');
    host.innerHTML = '';
    MONTH.dates.forEach(function (d) {
      var row = document.createElement('div');
      row.className = 'day';
      row.id = 'row-' + d.iso;

      var stamp = document.createElement('div');
      stamp.className = 'stamp';
      stamp.innerHTML = '<div class="num">' + d.day + '</div>' +
        '<div class="dow">' + d.dowLabel + '</div>' +
        (d.extra ? '<div class="ph">PH</div>' : '');
      row.appendChild(stamp);

      var seg = document.createElement('div');
      seg.className = 'seg';
      [['prefer', 'Prefer'], ['ok', 'Can round'], ['block', 'Block']].forEach(function (pair) {
        var b = document.createElement('button');
        b.type = 'button';
        b.className = 'v-' + pair[0];
        b.textContent = pair[1];
        b.setAttribute('aria-label', pair[1] + ' on ' + d.dowLabel + ' ' + d.day);
        b.addEventListener('click', function () { setValue(d.iso, pair[0]); });
        seg.appendChild(b);
      });
      row.appendChild(seg);
      host.appendChild(row);
    });
    paint();
  }

  function setValue(iso, value) {
    state[MONTH.key][iso] = value;
    paint();
    updateCount();
  }

  function paint() {
    MONTH.dates.forEach(function (d) {
      var row = document.getElementById('row-' + d.iso);
      var value = state[MONTH.key][d.iso];
      // The type class is reapplied here because paint() rewrites className
      // wholesale — drop it and choosing a day would strip its colour.
      row.className = 'day day--' + dayType(d) +
        (value === 'prefer' ? ' is-prefer' : value === 'block' ? ' is-block' : '');
      var buttons = row.querySelectorAll('.seg button');
      buttons[0].setAttribute('aria-pressed', value === 'prefer');
      buttons[1].setAttribute('aria-pressed', value === 'ok');
      buttons[2].setAttribute('aria-pressed', value === 'block');
    });
  }

  function updateCount() {
    var available = 0, prefer = 0;
    MONTH.dates.forEach(function (d) {
      if (state[MONTH.key][d.iso] !== 'block') available++;
      if (state[MONTH.key][d.iso] === 'prefer') prefer++;
    });

    document.getElementById('availNum').textContent = available + '/' + MONTH.dates.length;
    var lbl = 'days free in ' + MONTH.shortLabel +
      (prefer ? ' · ' + prefer + ' preferred' : '');
    var short = MONTH.target && available < MONTH.target;
    document.getElementById('availLbl').innerHTML = short
      ? lbl + ' <span class="warn">&mdash; below the &#8776;' + MONTH.target + ' average</span>'
      : lbl;

    document.getElementById('save').disabled = !document.getElementById('name').value;
  }

  /* ---------------- name ---------------- */

  function onNameChange() {
    var name = document.getElementById('name').value;
    var note = document.getElementById('prefillNote');

    DATA.months.forEach(function (m) {
      m.dates.forEach(function (d) { state[m.key][d.iso] = 'ok'; });
      extras[m.key] = { maxDays: '', notes: '' };
      saved[m.key] = null;
    });
    document.getElementById('maxDays').value = '';
    document.getElementById('notes').value = '';
    note.textContent = '';

    if (!name) { paint(); paintMonthTabs(); updateCount(); return; }

    note.textContent = 'Checking for earlier submissions…';
    apiGet('existing', { name: name }).then(function (byMonth) {
      var found = [];
      DATA.months.forEach(function (m) {
        var prev = byMonth ? byMonth[m.key] : null;
        if (!prev) return;
        saved[m.key] = prev.savedAt;
        found.push(m.shortLabel);
        prev.prefer.forEach(function (iso) {
          if (state[m.key][iso]) state[m.key][iso] = 'prefer';
        });
        prev.blocked.forEach(function (iso) {
          if (state[m.key][iso]) state[m.key][iso] = 'block';
        });
        extras[m.key] = {
          maxDays: prev.maxDays === null ? '' : prev.maxDays,
          notes: prev.notes
        };
      });

      document.getElementById('maxDays').value = extras[MONTH.key].maxDays;
      document.getElementById('notes').value = extras[MONTH.key].notes;
      note.textContent = found.length
        ? 'Loaded your saved answers for ' + found.join(' and ') + '. Saving replaces them.'
        : 'No submissions from you yet.';

      paint();
      paintMonthTabs();
      updateCount();
    }).catch(function () {
      note.textContent = 'Could not check earlier submissions. You can still save.';
      updateCount();
    });
  }

  /* ---------------- save ---------------- */

  function save() {
    var button = document.getElementById('save');
    var key = MONTH.key;
    var label = MONTH.shortLabel;
    stashExtras();

    button.disabled = true;
    button.textContent = 'Saving…';

    var prefer = [], blocked = [];
    MONTH.dates.forEach(function (d) {
      if (state[key][d.iso] === 'prefer') prefer.push(d.iso);
      if (state[key][d.iso] === 'block') blocked.push(d.iso);
    });

    var maxDays = extras[key].maxDays;

    apiPost({
      month: key,
      name: document.getElementById('name').value,
      prefer: prefer,
      blocked: blocked,
      maxDays: maxDays === '' ? null : Number(maxDays),
      notes: extras[key].notes
    })
      .then(function (res) {
        button.disabled = false;
        button.textContent = 'Save ' + MONTH.shortLabel;
        saved[key] = 'just now';
        paintMonthTabs();
        var others = DATA.months.filter(function (m) { return !saved[m.key]; });
        toast(label + ' saved.' + (others.length
          ? ' ' + others.map(function (m) { return m.shortLabel; }).join(' and ') +
            ' still to do — each month saves separately.'
          : ' Reopen this link any time to change it.'));
      })
      .catch(function (err) {
        button.disabled = false;
        button.textContent = 'Save ' + MONTH.shortLabel;
        toast(err.message, true);
      });
  }

  function toast(message, isError) {
    var el = document.getElementById('toast');
    el.textContent = message;
    el.className = 'toast' + (isError ? ' err' : '');
    el.style.display = 'block';
    setTimeout(function () { el.style.display = 'none'; }, 4500);
  }
</script>
</body>
</html>
