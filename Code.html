<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>সিলেবাস ট্র্যাকার — Syllabus Tracker</title>
  <style>
    :root{--bg:#0f1724;--card:#0b1220;--muted:#9aa6b2;--accent:#60a5fa;--glass:rgba(255,255,255,0.04)}
    *{box-sizing:border-box}
    body{margin:0;font-family:Inter, system-ui, -apple-system, "Noto Sans Bengali", Roboto, Arial, sans-serif;background:linear-gradient(180deg,#071228 0%, #071b2a 100%);color:#e6eef6;min-height:100vh;padding:28px}
    .wrap{max-width:1100px;margin:0 auto}
    header{display:flex;gap:16px;align-items:center;justify-content:space-between;margin-bottom:18px}
    h1{font-size:20px;margin:0}
    p.lead{margin:4px 0 0;color:var(--muted)}
    .controls{display:flex;gap:10px;align-items:center}
    button, .btn{background:var(--accent);color:#062639;border:none;padding:8px 12px;border-radius:8px;font-weight:600;cursor:pointer}
    .btn.ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted)}
    .grid{display:grid;grid-template-columns:1fr 320px;gap:18px;align-items:start}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:14px;border-radius:12px;border:1px solid rgba(255,255,255,0.03);box-shadow:0 6px 20px rgba(2,6,23,0.6)}
    .subject{margin-bottom:12px}
    summary{font-weight:700;font-size:16px;cursor:pointer}
    details{margin:12px 0;background:var(--glass);padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.03)}
    ul{list-style:none;padding:0;margin:8px 0 0}
    li{display:flex;align-items:center;gap:10px;padding:8px 6px;border-radius:8px}
    li:nth-child(odd){background:transparent}
    label{flex:1;cursor:pointer}
    .progress{height:10px;background:rgba(255,255,255,0.04);border-radius:999px;overflow:hidden}
    .progress > i{display:block;height:100%;width:0%;background:linear-gradient(90deg,#60a5fa,#34d399);transition:width .25s}
    .meta{font-size:13px;color:var(--muted);margin-top:8px}
    .sidebar .stat{display:flex;align-items:center;justify-content:space-between;padding:10px;border-radius:8px;background:rgba(255,255,255,0.02);margin-bottom:8px}
    .search{display:flex;gap:8px}
    input[type=search]{background:transparent;border:1px solid rgba(255,255,255,0.03);padding:8px;border-radius:8px;color:inherit;min-width:220px}
    .small{font-size:13px;color:var(--muted)}
    footer{margin-top:20px;color:var(--muted);font-size:13px;text-align:center}
    .actions{display:flex;gap:8px;flex-wrap:wrap}
    .hint{font-size:13px;color:var(--muted);margin-top:6px}
    @media(max-width:900px){.grid{grid-template-columns:1fr}.controls{flex-direction:column;align-items:flex-end}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div>
        <h1>📚 Syllabus Tracker</h1>
        <p class="lead"> Mark — Progress will be saved automatically</p>
      </div>
      <div class="controls">
        <div class="search card">
          <input id="searchInput" type="search" placeholder="Search chapters or tasks..." />
        </div>
        <div class="actions">
          <button id="exportBtn" title="Export progress">Export</button>
          <button id="importBtn" class="btn ghost" title="Import progress">Import</button>
          <input id="importFile" type="file" accept="application/json" style="display:none" />
          <button id="resetBtn" class="btn ghost">Reset</button>
        </div>
      </div>
    </header>

    <div class="grid">
      <main>
        <div id="syllabusContainer"></div>
      </main>

      <aside class="sidebar card">
        <div class="stat">
          <div>
            <div class="small">Overall Progress</div>
            <div id="overallPercent" style="font-weight:800;font-size:18px">0%</div>
          </div>
          <div style="width:110px">
            <div class="progress"><i id="overallBar"></i></div>
          </div>
        </div>
        <div class="meta">Quick tips</div>
        <ul class="hint">
          <li>🔖 Use search to quickly find chapters.</li>
          <li>💾 Progress is saved in your browser (localStorage).</li>
          <li>📤 Use Export to share progress or move to another device.</li>
        </ul>
      </aside>
    </div>

    <footer>Made for you — save the file as <code>index.html</code> and open it in your browser. Wanna upload to GitHub Pages? I can help 🚀</footer>
  </div>

  <script>
    // --- SYLLABUS DATA --- (generated from the list you provided)
    const SYLLABUS = [
      {
        subject: 'Physics 1st Paper',
        chapters: [
          { title: 'Chapter 01: ভৌত জগৎ ও পরিমাপ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 02: ভেক্টর', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 03: গতিবিদ্যা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 04: নিউটোনিয়ান বলবিদ্যা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 05: কাজ, শক্তি ও ক্ষমতা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 06: মহাকর্ষ ও অভিকর্ষ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 07: পদার্থের গাঠনিক ধর্ম', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 08: পর্যাবৃত্ত গতি', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 09: তরঙ্গ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 10: আদর্শ গ্যাস ও গ্যাসের গতিতত্ত্ব', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] }
        ]
      },
      {
        subject: 'Physics 2nd Paper',
        chapters: [
          { title: 'Chapter 01: তাপগতিবিদ্যা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 02: স্থির তড়িৎ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 03: চলতড়িৎ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 04: তড়িৎপ্রবাহের চৌম্বকক্রিয়া', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 05: তড়িৎ-চৌম্বকীয় আবেশ ও দিকপরিবর্তী প্রবাহ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 06: জ্যামিতিক আলোকবিজ্ঞান', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 07: ভৌত আলোকবিজ্ঞান', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 08: আধুনিক পদার্থবিজ্ঞানের সূচনা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 09: পরমাণুর মডেল এবং নিউক্লিয়ার পদার্থবিজ্ঞান', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 10: সেমিকন্ডাক্টর ও ইলেকট্রনিকস', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 11: জ্যোতির্বিজ্ঞান', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] }
        ]
      },
      {
        subject: 'Chemistry 1st Paper',
        chapters: [
          { title: 'Chapter 01: ল্যাবরেটরির নিরাপদ ব্যবহার', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 02: গুণগত রসায়ন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 03: মৌলের পর্যায়বৃত্ত ধর্ম ও রাসায়নিক বন্ধন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 04: রাসায়নিক পরিবর্তন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 05: কর্মমুখী রসায়ন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank', 'Engineering Question Bank'] }
        ]
      },
      {
        subject: 'Chemistry 2nd Paper',
        chapters: [
          { title: 'Chapter 01: পরিবেশ রসায়ন', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 02: জৈব রসায়ন', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 03: পরিমাণগত রসায়ন (Quantitative Chemistry)', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 04: তড়িৎ রসায়ন', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 05: অর্থনৈতিক রসায়ন', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] }
        ]
      },
      {
        subject: 'Higher Math 1st Paper',
        chapters: [
          { title: 'Chapter 01: ম্যাট্রিক্স ও নির্ণায়ক', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 02: ভেক্টর', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 03: সরলরেখা', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 04: বৃত্ত', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 05: বিন্যাস ও সমাবেশ', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 06: ত্রিকোণমিতিক অনুপাত', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 07: সংযুক্ত কোণের ত্রিকোণমিতিক অনুপাত', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 08: ফাংশন ও ফাংশনের লেখচিত্র', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 09: অন্তরীকরণ (Differentiation)', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 10: যোগজীকরণ (Integration)', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] }
        ]
      },
      {
        subject: 'Higher Math 2nd Paper',
        chapters: [
          { title: 'Chapter 01: বাস্তব সংখ্যা ও অসমতা', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 02: যোগাশ্রোয়ী প্রোগ্রাম', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 03: জটিল সংখ্যা', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 04: বহুপদী ও বহুপদী সমীকরণ', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 05: দ্বিপদী বিস্তৃতি', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 06: কণিক', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 07: বিপরীত ত্রিকোণমিতিক ফাংশন ও ত্রিকোণমিতিক সমীকরণ', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 08: স্থিতিবিদ্যা', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 09: সমতলে বস্তুকণার গতি', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] },
          { title: 'Chapter 10: বিস্তার পরিমাপ ও সম্ভবনা', tasks: ['Board CQ, MCQ', 'Varsity Question Bank', 'Engineering Question Bank'] }
        ]
      },
      {
        subject: 'Biology 1st Paper',
        chapters: [
          { title: 'Chapter 01: কোষ ও এর গঠন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 02: কোষ বিভাজন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 03: কোষ রসায়ন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 04: অণুজীব', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 05: শৈবাল ও ছত্রাক', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 06: ব্রায়োফাইটা ও টেরিডোফাইটা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 07: নগ্নবীজী ও আবৃতবীজী উদ্ভিদ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 08: টিস্যু ও টিস্যুতন্ত্র', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 09: উদ্ভিদ শারীরতত্ত্ব', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 10: উদ্ভিদ প্রজনন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 11: জীবপ্রযুক্তি', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 12: জীবের পরিবেশ, বিস্তার ও সংরক্ষণ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] }
        ]
      },
      {
        subject: 'Biology 2nd Paper',
        chapters: [
          { title: 'Chapter 01: প্রাণীর বিভিন্নতা ও শ্রেণিবিন্যাস', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 02: প্রাণীর পরিচিতি', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 03: পরিপাক ও শোষণ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 04: রক্ত সঞ্চালন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 05: শ্বাসক্রিয়া ও শ্বসন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 06: বর্জ্য ও নিষ্কাশন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 07: চলন ও অঙ্গচালনা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 08: সমন্বয় ও নিয়ন্ত্রণ', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 09: মানব জীবনের ধারাবাহিকতা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 10: মানবদেহের প্রতিরক্ষা', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] },
          { title: 'Chapter 11: জীনতত্ত্ব ও বিবর্তন', tasks: ['Board CQ, MCQ', 'Medical Question Bank', 'Varsity Question Bank'] }
        ]
      }
    ];

    // --- Storage helpers ---
    const STORAGE_KEY = 'syllabusTracker_v1';

    function loadState() {
      try{
        const raw = localStorage.getItem(STORAGE_KEY);
        return raw ? JSON.parse(raw) : {};
      }catch(e){console.warn('load error',e);return{}};
    }
    function saveState(state){localStorage.setItem(STORAGE_KEY, JSON.stringify(state));}

    // --- Rendering ---
    const container = document.getElementById('syllabusContainer');
    let state = loadState();

    function makeId(s,i,j,k){return `s${s}_c${i}_t${j}`}

    function render(){
      container.innerHTML = '';
      SYLLABUS.forEach((subject, sIdx)=>{
        const subjDiv = document.createElement('div');
        subjDiv.className = 'card subject';
        const subjHeader = document.createElement('div');
        subjHeader.style.display='flex';
        subjHeader.style.justifyContent='space-between';
        subjHeader.style.alignItems='center';
        subjHeader.innerHTML = `<strong>${subject.subject}</strong><div class='small' id='sub-progress-${sIdx}'>0%</div>`;
        subjDiv.appendChild(subjHeader);

        subject.chapters.forEach((chap, cIdx)=>{
          const d = document.createElement('details');
          d.open = false;
          const sum = document.createElement('summary');
          sum.textContent = chap.title;
          d.appendChild(sum);

          const progWrap = document.createElement('div');
          progWrap.className = 'progress';
          progWrap.style.marginTop = '8px';
          const progBar = document.createElement('i');
          progBar.style.width='0%';
          progBar.id = `prog-${sIdx}-${cIdx}`;
          progWrap.appendChild(progBar);
          d.appendChild(progWrap);

          const ul = document.createElement('ul');
          chap.tasks.forEach((task, tIdx)=>{
            const li = document.createElement('li');
            const id = makeId(sIdx,cIdx,tIdx);
            const checked = (state[id] === true);
            li.innerHTML = `<input type='checkbox' id='${id}' ${checked? 'checked':''} /> <label for='${id}'>${task}</label>`;
            ul.appendChild(li);
          });

          d.appendChild(ul);
          subjDiv.appendChild(d);
        });
        container.appendChild(subjDiv);
      });

      // attach events
      document.querySelectorAll('input[type=checkbox]').forEach(cb=>{
        cb.addEventListener('change', e=>{
          state[cb.id] = cb.checked;
          saveState(state);
          updateAllProgress();
        });
      });

      updateAllProgress();
    }

    function updateAllProgress(){
      // per chapter
      let totalTasks = 0, totalDone = 0;
      SYLLABUS.forEach((sub, sIdx)=>{
        let subTotal=0, subDone=0;
        sub.chapters.forEach((chap, cIdx)=>{
          const tasks = chap.tasks.length;
          subTotal += tasks;
          let done = 0;
          chap.tasks.forEach((t, tIdx)=>{
            const id = makeId(sIdx,cIdx,tIdx);
            if(state[id]) done++;
          });
          subDone += done;
          const pct = tasks? Math.round((done/tasks)*100):0;
          const bar = document.getElementById(`prog-${sIdx}-${cIdx}`);
          if(bar) bar.style.width = pct + '%';
        });
        // update subject percent display
        const subjPct = subTotal? Math.round((subDone/subTotal)*100):0;
        const subElem = document.getElementById(`sub-progress-${sIdx}`);
        if(subElem) subElem.textContent = subjPct + '%';
        totalTasks += subTotal; totalDone += subDone;
      });
      const overallPct = totalTasks? Math.round((totalDone/totalTasks)*100):0;
      document.getElementById('overallPercent').textContent = overallPct + '%';
      document.getElementById('overallBar').style.width = overallPct + '%';
    }

    // --- Search ---
    const searchInput = document.getElementById('searchInput');
    searchInput.addEventListener('input', ()=>{
      const q = searchInput.value.trim().toLowerCase();
      document.querySelectorAll('#syllabusContainer .subject').forEach((sub, sIdx)=>{
        let anySubVisible = false;
        sub.querySelectorAll('details').forEach((d, cIdx)=>{
          const title = d.querySelector('summary').textContent.toLowerCase();
          const items = Array.from(d.querySelectorAll('label')).map(l=>l.textContent.toLowerCase()).join(' ');
          const match = !q || title.includes(q) || items.includes(q);
          d.style.display = match? 'block':'none';
          if(match) anySubVisible = true;
        });
        sub.style.display = anySubVisible? 'block':'none';
      });
    });

    // --- Export / Import / Reset ---
    document.getElementById('exportBtn').addEventListener('click', ()=>{
      const dataStr = JSON.stringify(state);
      const blob = new Blob([dataStr],{type:'application/json'});
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url; a.download = 'syllabus-progress.json';
      document.body.appendChild(a); a.click(); a.remove(); URL.revokeObjectURL(url);
    });

    const importFile = document.getElementById('importFile');
    document.getElementById('importBtn').addEventListener('click', ()=>importFile.click());
    importFile.addEventListener('change', e=>{
      const f = e.target.files[0];
      if(!f) return;
      const reader = new FileReader();
      reader.onload = ev=>{
        try{
          const obj = JSON.parse(ev.target.result);
          state = obj; saveState(state); render();
          alert('Imported progress ✅');
        }catch(err){alert('Invalid file');}
      };
      reader.readAsText(f);
      importFile.value = null;
    });

    document.getElementById('resetBtn').addEventListener('click', ()=>{
      if(confirm('Reset all progress?')){ state = {}; saveState(state); render(); }
    });

    // initial render
    render();
  </script>
</body>
</html>