<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>WebTagio — Tag Everything on the Web</title>
<style>
  :root{
    --bg:#0f1720; --card:#0b1220; --muted:#98a2b3; --accent:#6ee7b7;
    --glass: rgba(255,255,255,0.03);
    --radius:12px; --gap:16px; --maxw:1100px;
    font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    color-scheme: dark;
  }
  html,body{height:100%}
  body{
    margin:0; background:linear-gradient(180deg,#071025 0%, #07101a 100%);
    color:#e6eef6; display:flex; align-items:flex-start; justify-content:center;
    padding:28px; -webkit-font-smoothing:antialiased;
  }
  .app{
    width:100%; max-width:var(--maxw);
    display:grid; grid-template-columns: 360px 1fr; gap:24px;
  }
  header{
    grid-column:1/-1; display:flex; align-items:center; justify-content:space-between;
    gap:12px; margin-bottom:6px;
  }
  .brand {display:flex; align-items:center; gap:12px}
  .logo{
    width:44px;height:44px;border-radius:10px;background:linear-gradient(135deg,#0ea5a4,#7c3aed);
    display:flex;align-items:center;justify-content:center;font-weight:700;color:white;
    box-shadow:0 6px 18px rgba(0,0,0,0.6);
  }
  h1{font-size:16px;margin:0}
  p.lead{margin:0;color:var(--muted);font-size:13px}
  .controls{display:flex; gap:10px; align-items:center}
  button, .chip{
    background:var(--glass); border:1px solid rgba(255,255,255,0.03); color:inherit;
    padding:8px 12px; border-radius:10px; cursor:pointer; font-size:13px;
  }
  .left{
    background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    padding:16px; border-radius:var(--radius); height:calc(100vh - 140px); overflow:auto;
  }
  .form-row{display:flex; gap:8px; margin-bottom:10px}
  label{font-size:12px;color:var(--muted);display:block;margin-bottom:6px}
  input[type="text"], textarea{
    width:100%; padding:10px; border-radius:8px; background:transparent; border:1px solid rgba(255,255,255,0.04);
    color:inherit; outline:none; font-size:13px;
  }
  textarea{ min-height:84px; resize:vertical}
  .tag-input{display:flex; gap:8px; flex-wrap:wrap; align-items:center}
  .tag-chip{background:rgba(255,255,255,0.03); padding:6px 8px; border-radius:999px; font-size:12px;}
  .add-btn{background:linear-gradient(90deg,#10b981,#06b6d4); color:#042018; border:none}
  .right{
    height:calc(100vh - 140px); overflow:auto;
  }
  .searchbar{display:flex; gap:8px; align-items:center; margin-bottom:12px}
  .searchbar input{flex:1; padding:12px; border-radius:12px; font-size:14px; border:none; background:rgba(255,255,255,0.03)}
  .filters{display:flex; gap:8px; flex-wrap:wrap; margin-bottom:14px}
  .cards{display:grid; grid-template-columns: repeat(auto-fill, minmax(220px,1fr)); gap:14px}
  .card{
    background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
    padding:14px; border-radius:12px; min-height:120px; display:flex; flex-direction:column; gap:10px;
    border:1px solid rgba(255,255,255,0.02);
  }
  .card .meta{display:flex; gap:12px; align-items:center}
  .avatar{
    width:44px;height:44px;border-radius:10px;display:flex;align-items:center;justify-content:center;font-weight:700;
    color:#022; background:linear-gradient(135deg,#8b5cf6,#06b6d4); flex-shrink:0;
  }
  .title{font-weight:600; font-size:14px;}
  .url{font-size:12px;color:var(--muted);overflow:hidden;text-overflow:ellipsis;white-space:nowrap}
  .tag-list{display:flex; gap:6px; flex-wrap:wrap}
  .tag-pill{background:rgba(255,255,255,0.03); padding:6px 8px; border-radius:999px; font-size:12px; color:var(--muted)}
  .notes{font-size:13px;color:var(--muted); margin-top:6px; overflow:hidden; max-height:56px}
  .small{font-size:12px;color:var(--muted)}
  .empty{padding:36px;border-radius:12px;background:rgba(255,255,255,0.02); text-align:center; color:var(--muted)}
  footer{grid-column:1/-1; margin-top:8px; color:var(--muted); font-size:12px; text-align:center}
  /* responsive */
  @media (max-width:900px){
    .app{grid-template-columns:1fr; padding-bottom:30px}
    .left{height:auto}
    .right{height:auto}
  }
</style>
</head>
<body>
  <div class="app" id="app">
    <header>
      <div class="brand">
        <div class="logo">#W</div>
        <div>
          <h1>WebTagio</h1>
          <p class="lead">Personal offline bookmark manager</p>
        </div>
      </div>

      <div class="controls">
        <button id="exportBtn">Export JSON</button>
        <button id="importBtn">Import JSON</button>
        <input id="fileInput" type="file" accept="application/json" style="display:none" />
        <button id="clearBtn" title="Delete all data">Clear All</button>
      </div>
    </header>

    <aside class="left" aria-label="Add bookmarks and filters">
      <div>
        <label for="urlInput">URL</label>
        <input id="urlInput" type="text" placeholder="https://example.com" />
      </div>

      <div class="form-row">
        <div style="flex:1">
          <label for="nameInput">Name</label>
          <input id="nameInput" type="text" placeholder="Example - Marketing article" />
        </div>
      </div>

      <div>
        <label for="tagsInput">Tags (comma separated)</label>
        <input id="tagsInput" type="text" placeholder="news, research, recipes" />
      </div>

      <div>
        <label for="notesInput">Notes</label>
        <textarea id="notesInput" placeholder="Short notes about this bookmark"></textarea>
      </div>

      <div style="display:flex; gap:8px; margin-top:12px; align-items:center;">
        <button id="addBtn" class="add-btn">Add Bookmark</button>
        <div style="flex:1"></div>
        <div class="small" id="countLabel">0 bookmarks</div>
      </div>

      <hr style="border:none;height:1px;background:rgba(255,255,255,0.02);margin:16px 0" />

      <div style="margin-bottom:8px">
        <label>Quick filters</label>
        <div style="display:flex; gap:8px; margin-top:8px; flex-wrap:wrap">
          <button class="chip" data-kind="recent" id="filterRecent">Recent</button>
          <button class="chip" data-kind="today" id="filterToday">Today</button>
          <button class="chip" data-kind="hasnotes" id="filterNotes">Has notes</button>
        </div>
      </div>

      <div style="margin-top:16px">
        <label>Tags</label>
        <div id="tagCloud" style="margin-top:10px;display:flex;gap:8px;flex-wrap:wrap"></div>
      </div>

      <div style="margin-top:20px">
        <label>Search tips</label>
        <p class="small" style="margin-top:6px;color:var(--muted)">Use keywords, multiple terms (AND), or exact phrase using quotes. Click tags to filter.</p>
      </div>

    </aside>

    <main class="right">
      <div class="searchbar">
        <input id="searchBox" placeholder="Search bookmarks (name, url, tags, notes)... ⌘/ to focus" />
        <select id="sortSelect" style="padding:10px;border-radius:10px;background:transparent;border:1px solid rgba(255,255,255,0.03)">
          <option value="relevance">Best match</option>
          <option value="newest">Newest</option>
          <option value="oldest">Oldest</option>
          <option value="name">Name (A→Z)</option>
        </select>
      </div>

      <div class="filters" id="activeFilters"></div>

      <div id="resultArea">
        <div class="cards" id="cards"></div>
      </div>
    </main>

    <footer>WebTagio — lightweight • data stored locally • Export/Import easily</footer>
  </div>

<script>
/* ======= IndexedDB wrapper (promises) ======= */
const DB_NAME = 'webtagio_v1';
const STORE = 'bookmarks';
const IDX_STORE = 'invertedIndex';

function openDB(){
  return new Promise((resolve, reject) => {
    const req = indexedDB.open(DB_NAME, 1);
    req.onupgradeneeded = (ev) => {
      const db = ev.target.result;
      if(!db.objectStoreNames.contains(STORE)){
        const s = db.createObjectStore(STORE, { keyPath: 'id' });
        s.createIndex('created_at', 'created_at', { unique: false });
      }
      if(!db.objectStoreNames.contains(IDX_STORE)){
        db.createObjectStore(IDX_STORE, { keyPath: 'token' });
      }
    };
    req.onsuccess = () => resolve(req.result);
    req.onerror = () => reject(req.error);
  });
}

async function idbPut(storeName, value){
  const db = await openDB();
  return new Promise((res, rej) => {
    const tx = db.transaction([storeName], 'readwrite');
    tx.objectStore(storeName).put(value);
    tx.oncomplete = () => res(true);
    tx.onerror = () => rej(tx.error);
  });
}

async function idbGet(storeName, key){
  const db = await openDB();
  return new Promise((res, rej) => {
    const tx = db.transaction([storeName], 'readonly');
    const r = tx.objectStore(storeName).get(key);
    r.onsuccess = () => res(r.result);
    r.onerror = () => rej(r.error);
  });
}

async function idbDelAll(storeName){
  const db = await openDB();
  return new Promise((res, rej) => {
    const tx = db.transaction([storeName], 'readwrite');
    tx.objectStore(storeName).clear();
    tx.oncomplete = () => res();
    tx.onerror = () => rej(tx.error);
  });
}

async function idbGetAll(storeName){
  const db = await openDB();
  return new Promise((res, rej) => {
    const tx = db.transaction([storeName], 'readonly');
    const r = tx.objectStore(storeName).getAll();
    r.onsuccess = () => res(r.result || []);
    r.onerror = () => rej(r.error);
  });
}

async function idbGetAllKeys(storeName){
  const db = await openDB();
  return new Promise((res, rej) => {
    const tx = db.transaction([storeName], 'readonly');
    const r = tx.objectStore(storeName).getAllKeys();
    r.onsuccess = () => res(r.result || []);
    r.onerror = () => rej(r.error);
  });
}

/* ======= Bookmark + index logic ======= */

function uid(){ // short unique id
  return 'b_' + Math.random().toString(36).slice(2,10);
}

function normalizeText(s){
  return (s||'').toString().toLowerCase();
}

function tokenize(s){
  if(!s) return [];
  // keep words, numbers, split on non-word
  return normalizeText(s).split(/[^a-z0-9]+/).filter(Boolean);
}

// store: token -> { token, ids: [id, ...] }
async function indexAdd(tokens, id){
  const db = await openDB();
  return new Promise((resolve, reject) => {
    const tx = db.transaction([IDX_STORE], 'readwrite');
    const idx = tx.objectStore(IDX_STORE);
    const uniqueTokens = Array.from(new Set(tokens));
    let pending = uniqueTokens.length;
    if(pending === 0){ resolve(true); return; }
    uniqueTokens.forEach(token => {
      const req = idx.get(token);
      req.onsuccess = () => {
        const cur = req.result;
        const ids = cur ? new Set(cur.ids) : new Set();
        ids.add(id);
        idx.put({ token, ids: Array.from(ids) });
        pending--; if(pending===0) resolve(true);
      };
      req.onerror = () => { pending--; if(pending===0) resolve(true); };
    });
    tx.onerror = () => reject(tx.error);
  });
}

async function indexRemoveById(id){
  const db = await openDB();
  return new Promise((resolve, reject) => {
    const tx = db.transaction([IDX_STORE], 'readwrite');
    const idx = tx.objectStore(IDX_STORE);
    // iterate all tokens, remove id from arrays (relatively fast for small datasets)
    const cursor = idx.openCursor();
    cursor.onsuccess = (ev) => {
      const c = ev.target.result;
      if(!c){ resolve(true); return; }
      const rec = c.value;
      const newIds = (rec.ids || []).filter(x => x !== id);
      if(newIds.length === 0) c.delete();
      else c.update({ token: rec.token, ids: newIds });
      c.continue();
    };
    cursor.onerror = () => reject(cursor.error);
  });
}

async function indexSearchTokens(tokens){
  if(!tokens || tokens.length===0) return [];
  const db = await openDB();
  return new Promise((resolve, reject) => {
    const tx = db.transaction([IDX_STORE], 'readonly');
    const idx = tx.objectStore(IDX_STORE);
    let results = null;
    let pending = tokens.length;
    tokens.forEach(t => {
      const req = idx.get(t);
      req.onsuccess = () => {
        const rec = req.result;
        const ids = rec ? rec.ids : [];
        if(results === null) results = new Set(ids);
        else results = new Set([...results].filter(x => ids.includes(x)));
        pending--; if(pending===0) resolve(Array.from(results || []));
      };
      req.onerror = () => { pending--; if(pending===0) resolve(Array.from(results || [])); };
    });
  });
}

/* ======= App state & UI ======= */

const $ = sel => document.querySelector(sel);
const $$ = sel => Array.from(document.querySelectorAll(sel));

const urlInput = $('#urlInput');
const nameInput = $('#nameInput');
const tagsInput = $('#tagsInput');
const notesInput = $('#notesInput');
const addBtn = $('#addBtn');
const cardsEl = $('#cards');
const searchBox = $('#searchBox');
const sortSelect = $('#sortSelect');
const countLabel = $('#countLabel');
const tagCloud = $('#tagCloud');
const exportBtn = $('#exportBtn');
const importBtn = $('#importBtn');
const fileInput = $('#fileInput');
const importButton = $('#importBtn');
const clearBtn = $('#clearBtn');
const activeFilters = $('#activeFilters');

let activeTagFilters = new Set();
let activeQuickFilter = null;

async function addBookmarkFromForm(){
  const url = (urlInput.value||'').trim();
  if(!url) { alert('Please enter a URL'); urlInput.focus(); return; }
  const name = (nameInput.value || '').trim() || url;
  const tags = (tagsInput.value||'').split(',').map(s=>s.trim()).filter(Boolean);
  const notes = (notesInput.value||'').trim();
  const created_at = new Date().toISOString();
  const id = uid();
  const bm = { id, url, name, tags, notes, created_at };
  await idbPut(STORE, bm);
  // build tokens: url, name, tags, notes
  const tokens = [
    ...tokenize(name),
    ...tokenize(url),
    ...tags.flatMap(t => tokenize(t)),
    ...tokenize(notes)
  ];
  await indexAdd(tokens, id);
  clearForm();
  await render();
}

function clearForm(){
  urlInput.value=''; nameInput.value=''; tagsInput.value=''; notesInput.value='';
  urlInput.focus();
}

function domainFromUrl(u){
  try{
    const url = new URL(u);
    return url.hostname.replace('www.','');
  }catch(e){
    return u;
  }
}

function avatarText(name, url){
  if(name && name.length) return name.trim()[0].toUpperCase();
  const d = domainFromUrl(url);
  return d ? d[0].toUpperCase() : '?';
}

function timeAgo(iso){
  const d = new Date(iso);
  const diff = Date.now() - d.getTime();
  const min = Math.round(diff/60000);
  if(min < 1) return 'just now';
  if(min < 60) return `${min}m`;
  const hr = Math.round(min/60);
  if(hr < 24) return `${hr}h`;
  const days = Math.round(hr/24);
  if(days < 30) return `${days}d`;
  return d.toLocaleDateString();
}

async function loadAllBookmarks(){
  return await idbGetAll(STORE);
}

function scoreAndSort(results, queryTokens, sortMode){
  // results are array of bookmark objects
  // compute a simple score: matches count + recency boost
  const qset = new Set(queryTokens || []);
  return results.map(r => {
    const tokens = new Set([
      ...tokenize(r.name), ...tokenize(r.url), ...r.tags.flatMap(t=>tokenize(t)), ...tokenize(r.notes)
    ]);
    let matchCount = 0;
    qset.forEach(q => { if(tokens.has(q)) matchCount++; });
    const age = Date.now() - new Date(r.created_at).getTime();
    const recency = Math.max(0, 1 - age / (1000*60*60*24*365)); // 0..1
    const score = matchCount + recency;
    return { r, score };
  }).sort((a,b) => {
    if(sortMode === 'newest') return new Date(b.r.created_at) - new Date(a.r.created_at);
    if(sortMode === 'oldest') return new Date(a.r.created_at) - new Date(b.r.created_at);
    if(sortMode === 'name') return a.r.name.localeCompare(b.r.name);
    // relevance fallback
    if(b.score !== a.score) return b.score - a.score;
    return new Date(b.r.created_at) - new Date(a.r.created_at);
  }).map(x => x.r);
}

function renderCard(b){
  const div = document.createElement('div');
  div.className = 'card';
  div.dataset.id = b.id;
  div.innerHTML = `
    <div class="meta">
      <div class="avatar" aria-hidden="true">${avatarText(b.name,b.url)}</div>
      <div style="flex:1">
        <div class="title">${escapeHtml(b.name)}</div>
        <div class="url">${escapeHtml(b.url)}</div>
      </div>
      <div style="text-align:right">
        <div class="small">${timeAgo(b.created_at)}</div>
        <div style="margin-top:6px">
          <button data-action="open" class="chip">Open</button>
          <button data-action="del" class="chip">Delete</button>
        </div>
      </div>
    </div>
    <div class="tag-list">${b.tags.map(t=>`<span class="tag-pill">${escapeHtml(t)}</span>`).join('')}</div>
    ${b.notes ? `<div class="notes">${escapeHtml(b.notes)}</div>` : ''}
  `;
  // open and delete handlers
  div.querySelectorAll('button[data-action]').forEach(btn => {
    btn.addEventListener('click', async (ev) => {
      const act = btn.dataset.action;
      if(act === 'open') window.open(b.url, '_blank');
      if(act === 'del'){
        if(!confirm(`Delete bookmark "${b.name}"?`)) return;
        await idbDelAll?._noop; // noop
        await deleteBookmark(b.id);
        await render();
      }
    });
  });
  // tag click to filter
  div.querySelectorAll('.tag-pill').forEach(el => {
    el.addEventListener('click', (ev)=>{
      const tag = el.textContent;
      toggleTagFilter(tag);
    });
  });
  return div;
}

async function deleteBookmark(id){
  // remove bookmark and remove id from index
  const db = await openDB();
  return new Promise((resolve, reject) => {
    const tx = db.transaction([STORE, IDX_STORE], 'readwrite');
    tx.objectStore(STORE).delete(id);
    // remove id from all index tokens
    const idx = tx.objectStore(IDX_STORE);
    const cursor = idx.openCursor();
    cursor.onsuccess = (ev) => {
      const c = ev.target.result;
      if(!c) return;
      const rec = c.value;
      const newIds = (rec.ids||[]).filter(x => x !== id);
      if(newIds.length === 0) c.delete();
      else c.update({ token: rec.token, ids: newIds });
      c.continue();
    };
    tx.oncomplete = () => resolve(true);
    tx.onerror = () => reject(tx.error);
  });
}

function escapeHtml(text){
  return String(text || '').replace(/[&<>"']/g, s => ({'&':'&amp;','<':'&lt;','>':'&gt;','"':'&quot;',"'":'&#39;'}[s]));
}

function parseQuery(q){
  q = (q||'').trim();
  if(!q) return [];
  // support phrase queries in quotes AND simple tokens
  const phraseMatches = Array.from(q.matchAll(/"([^"]+)"/g)).map(m => m[1]);
  const withoutPhrases = q.replace(/"[^"]+"/g, ' ');
  const tokens = tokenize(phraseMatches.join(' ') + ' ' + withoutPhrases);
  return tokens;
}

async function runSearchAndFilter(){
  const q = searchBox.value.trim();
  const tokens = parseQuery(q);
  let ids = null;
  if(tokens.length > 0){
    ids = await indexSearchTokens(tokens);
  } else {
    ids = await idbGetAllKeys(STORE);
  }
  // get objects for these ids
  const all = await loadAllBookmarks();
  const map = new Map(all.map(x => [x.id, x]));
  let results = ids.map(id => map.get(id)).filter(Boolean);

  // apply tag filters
  if(activeTagFilters.size){
    results = results.filter(r => r.tags.some(t => activeTagFilters.has(t)));
  }
  // quick filters
  if(activeQuickFilter === 'hasnotes'){
    results = results.filter(r => (r.notes||'').trim().length>0);
  }
  if(activeQuickFilter === 'today'){
    const start = new Date(); start.setHours(0,0,0,0);
    results = results.filter(r => new Date(r.created_at) >= start);
  }
  if(activeQuickFilter === 'recent'){
    const cutoff = Date.now() - (1000*60*60*24*7); // 7 days
    results = results.filter(r => new Date(r.created_at).getTime() >= cutoff);
  }

  // sort & score
  const sorted = scoreAndSort(results, tokens, sortSelect.value);
  return sorted;
}

async function render(){
  const results = await runSearchAndFilter();
  cardsEl.innerHTML = '';
  if(results.length === 0){
    cardsEl.innerHTML = `<div class="empty">No bookmarks yet — add one from the left. Tip: try "recent" filter or add tags.</div>`;
  } else {
    const frag = document.createDocumentFragment();
    results.forEach(b => frag.appendChild(renderCard(b)));
    cardsEl.appendChild(frag);
  }
  // update tag cloud and count
  const all = await loadAllBookmarks();
  countLabel.textContent = `${all.length} bookmarks`;
  renderTagCloud(all);
  renderActiveFilters();
}

function renderTagCloud(list){
  const tagCount = new Map();
  list.forEach(b => b.tags.forEach(t => tagCount.set(t, (tagCount.get(t)||0)+1)));
  const items = Array.from(tagCount.entries()).sort((a,b)=>b[1]-a[1]);
  tagCloud.innerHTML = items.map(([t,c]) => `<button class="chip tag-chip" data-tag="${escapeHtml(t)}">${escapeHtml(t)} <span style="opacity:.6">(${c})</span></button>`).join('');
  tagCloud.querySelectorAll('.tag-chip').forEach(btn => {
    btn.addEventListener('click', () => toggleTagFilter(btn.dataset.tag));
  });
}

function toggleTagFilter(tag){
  if(activeTagFilters.has(tag)) activeTagFilters.delete(tag);
  else activeTagFilters.add(tag);
  render();
}

function renderActiveFilters(){
  activeFilters.innerHTML = '';
  if(activeQuickFilter){
    const el = document.createElement('div');
    el.className='chip';
    el.textContent = activeQuickFilter;
    el.addEventListener('click', ()=>{ activeQuickFilter=null; render(); });
    activeFilters.appendChild(el);
  }
  activeTagFilters.forEach(t => {
    const el = document.createElement('div');
    el.className='chip';
    el.textContent = t;
    el.addEventListener('click', ()=>{ activeTagFilters.delete(t); render(); });
    activeFilters.appendChild(el);
  });
}

/* ======= Export / Import / Clear ======= */
exportBtn.addEventListener('click', async ()=>{
  const all = await idbGetAll(STORE);
  const data = { exported_at: new Date().toISOString(), bookmarks: all };
  const blob = new Blob([JSON.stringify(data, null, 2)], { type: 'application/json' });
  const url = URL.createObjectURL(blob);
  const a = document.createElement('a');
  a.href = url; a.download = `webtagio-backup-${(new Date()).toISOString().slice(0,19).replaceAll(':','-')}.json`;
  document.body.appendChild(a); a.click(); a.remove();
  URL.revokeObjectURL(url);
});

importBtn.addEventListener('click', ()=> fileInput.click());
fileInput.addEventListener('change', async (ev)=>{
  const f = ev.target.files[0]; if(!f) return;
  const text = await f.text();
  try{
    const parsed = JSON.parse(text);
    if(!parsed.bookmarks) throw new Error('Invalid file');
    // merge: add entries with new ids if collision
    for(const b of parsed.bookmarks){
      const newId = b.id || uid();
      const bm = { id: newId, url: b.url||'', name: b.name||b.url||'', tags: b.tags||[], notes: b.notes||'', created_at: b.created_at||new Date().toISOString() };
      await idbPut(STORE, bm);
      const tokens = [...tokenize(bm.name), ...tokenize(bm.url), ...bm.tags.flatMap(t=>tokenize(t)), ...tokenize(bm.notes)];
      await indexAdd(tokens, bm.id);
    }
    alert('Import complete');
    fileInput.value='';
    render();
  }catch(e){
    alert('Import failed: ' + (e.message||e));
  }
});

clearBtn.addEventListener('click', async ()=>{
  if(!confirm('This will delete ALL bookmarks and indexes. Continue?')) return;
  await idbDelAll(STORE);
  await idbDelAll(IDX_STORE);
  alert('All data cleared');
  render();
});

/* ======= Quick filters === */
$('#filterNotes').addEventListener('click', ()=> { activeQuickFilter = activeQuickFilter==='hasnotes' ? null : 'hasnotes'; render(); });
$('#filterToday').addEventListener('click', ()=> { activeQuickFilter = activeQuickFilter==='today' ? null : 'today'; render(); });
$('#filterRecent').addEventListener('click', ()=> { activeQuickFilter = activeQuickFilter==='recent' ? null : 'recent'; render(); });

/* ======= Add / Search handlers === */
addBtn.addEventListener('click', addBookmarkFromForm);
[nameInput, urlInput, tagsInput, notesInput].forEach(el => el.addEventListener('keydown', (e)=>{
  if(e.key === 'Enter' && (e.metaKey || e.ctrlKey)){
    addBookmarkFromForm();
  }
}));

searchBox.addEventListener('input', debounce(()=>{ render(); }, 150));
sortSelect.addEventListener('change', render);

/* keyboard focus shortcut: Cmd/Control + / */
document.addEventListener('keydown', (e)=>{
  if((e.ctrlKey || e.metaKey) && e.key === '/'){ e.preventDefault(); searchBox.focus(); searchBox.select(); }
});

/* ======= Utilities ======= */

function debounce(fn, ms=200){
  let t;
  return (...a)=>{ clearTimeout(t); t=setTimeout(()=>fn(...a), ms); };
}

async function init(){
  // ensure DB exists
  await openDB();
  // initial render
  render();
  // attempt to focus URL
  urlInput.focus();
}

init();

/* polyfills for clearing index store via idbDelAll */
async function idbDelAllConsidered(name){
  return idbDelAll(name);
}
</script>
</body>
</html>
