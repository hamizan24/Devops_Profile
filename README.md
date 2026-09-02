
<style>
  .container { padding: 1rem 0; font-family: var(--font-mono); }
  .hero { background: var(--surface-1); border: 0.5px solid var(--border); border-radius: 12px; padding: 1.25rem; margin-bottom: 1rem; }
  .name { font-size: 22px; font-weight: 500; color: var(--text-primary); margin: 0 0 4px; font-family: var(--font-sans); }
  .title-tag { display: inline-block; background: var(--bg-accent); color: var(--text-accent); font-size: 12px; padding: 3px 10px; border-radius: var(--radius); margin: 4px 2px; font-family: var(--font-sans); }
  .section { margin-bottom: 1rem; }
  .section-title { font-size: 13px; font-weight: 500; color: var(--text-secondary); text-transform: uppercase; letter-spacing: 0.08em; margin-bottom: 8px; font-family: var(--font-sans); }
  .skill-row { display: flex; align-items: center; gap: 10px; margin-bottom: 6px; }
  .skill-label { font-size: 13px; color: var(--text-primary); min-width: 120px; font-family: var(--font-sans); }
  .skill-bar-bg { flex: 1; height: 6px; background: var(--surface-0); border-radius: 99px; overflow: hidden; }
  .skill-bar-fill { height: 100%; border-radius: 99px; }
  .skill-pct { font-size: 12px; color: var(--text-muted); min-width: 32px; text-align: right; font-family: var(--font-sans); }
  .badge { display: inline-flex; align-items: center; gap: 4px; font-size: 11px; padding: 3px 8px; border-radius: var(--radius); border: 0.5px solid var(--border); color: var(--text-secondary); margin: 2px; font-family: var(--font-sans); }
  .project-card { background: var(--surface-2); border: 0.5px solid var(--border); border-radius: 12px; padding: 1rem 1.25rem; margin-bottom: 8px; }
  .project-name { font-size: 15px; font-weight: 500; color: var(--text-accent); margin: 0 0 4px; font-family: var(--font-sans); }
  .project-desc { font-size: 13px; color: var(--text-secondary); margin: 0 0 8px; font-family: var(--font-sans); line-height: 1.5; }
  .tag { display: inline-block; background: var(--bg-success); color: var(--text-success); font-size: 11px; padding: 2px 7px; border-radius: var(--radius); margin: 2px; font-family: var(--font-sans); }
  .copy-btn { width: 100%; margin-top: 1rem; padding: 10px; font-size: 13px; font-family: var(--font-sans); cursor: pointer; border-radius: var(--radius); }
  .divider { border: none; border-top: 0.5px solid var(--border); margin: 1rem 0; }
  .stat-row { display: grid; grid-template-columns: repeat(2, minmax(0,1fr)); gap: 8px; margin-bottom: 1rem; }
  .stat-card { background: var(--surface-1); border-radius: var(--radius); padding: 0.75rem 1rem; }
  .stat-num { font-size: 20px; font-weight: 500; color: var(--text-primary); font-family: var(--font-sans); }
  .stat-lbl { font-size: 12px; color: var(--text-muted); font-family: var(--font-sans); }
  .tab-row { display: flex; gap: 0; border: 0.5px solid var(--border); border-radius: var(--radius); overflow: hidden; margin-bottom: 1rem; }
  .tab { flex: 1; padding: 8px 4px; font-size: 12px; text-align: center; cursor: pointer; border: none; background: var(--surface-1); color: var(--text-secondary); font-family: var(--font-sans); transition: background 0.15s; }
  .tab.active { background: var(--bg-accent); color: var(--text-accent); font-weight: 500; }
  .panel { display: none; }
  .panel.active { display: block; }
</style>
<div class="container">
  <h2 class="sr-only">GitLab README preview for Ijan — DevOps Engineer profile</h2>

  <div class="hero">
    <div style="display:flex; align-items:center; gap:12px; margin-bottom:10px;">
      <div style="width:44px;height:44px;border-radius:50%;background:var(--bg-accent);display:flex;align-items:center;justify-content:center;font-weight:500;font-size:15px;color:var(--text-accent);font-family:var(--font-sans);">IJ</div>
      <div>
        <p class="name">Ijan</p>
        <p style="font-size:12px;color:var(--text-muted);margin:0;font-family:var(--font-sans);">Selangor, Malaysia</p>
      </div>
    </div>
    <div>
      <span class="title-tag">IT → DevOps</span>
      <span class="title-tag">Infrastructure</span>
      <span class="title-tag">Ops.Nexus Data</span>
    </div>
    <p style="font-size:13px;color:var(--text-secondary);margin:10px 0 0;font-family:var(--font-sans);line-height:1.6;">
      IT Support Engineer transitioning into DevOps. Building real pipelines, automating infrastructure, and shipping reliable systems.
    </p>
  </div>

  <div class="tab-row" role="tablist">
    <button class="tab active" onclick="showTab('skills')" aria-selected="true">Skills</button>
    <button class="tab" onclick="showTab('projects')" aria-selected="false">Projects</button>
    <button class="tab" onclick="showTab('stats')" aria-selected="false">Stats</button>
    <button class="tab" onclick="showTab('readme')" aria-selected="false">README</button>
  </div>

  <div id="tab-skills" class="panel active">
    <div class="section">
      <div class="section-title">Core Skills</div>
      <div class="skill-row">
        <span class="skill-label"><i class="ti ti-git-branch" aria-hidden="true"></i> CI/CD</span>
        <div class="skill-bar-bg"><div class="skill-bar-fill" style="width:82%;background:#185FA5;"></div></div>
        <span class="skill-pct">82%</span>
      </div>
      <div class="skill-row">
        <span class="skill-label"><i class="ti ti-box" aria-hidden="true"></i> Docker/K8s</span>
        <div class="skill-bar-bg"><div class="skill-bar-fill" style="width:75%;background:#0F6E56;"></div></div>
        <span class="skill-pct">75%</span>
      </div>
      <div class="skill-row">
        <span class="skill-label"><i class="ti ti-server" aria-hidden="true"></i> Terraform</span>
        <div class="skill-bar-bg"><div class="skill-bar-fill" style="width:68%;background:#854F0B;"></div></div>
        <span class="skill-pct">68%</span>
      </div>
      <div class="skill-row">
        <span class="skill-label"><i class="ti ti-terminal" aria-hidden="true"></i> Linux/Bash</span>
        <div class="skill-bar-bg"><div class="skill-bar-fill" style="width:88%;background:#3C3489;"></div></div>
        <span class="skill-pct">88%</span>
      </div>
      <div class="skill-row">
        <span class="skill-label"><i class="ti ti-chart-line" aria-hidden="true"></i> Monitoring</span>
        <div class="skill-bar-bg"><div class="skill-bar-fill" style="width:70%;background:#993C1D;"></div></div>
        <span class="skill-pct">70%</span>
      </div>
    </div>
    <hr class="divider">
    <div class="section-title">Tech Stack</div>
    <div>
      <span class="badge"><i class="ti ti-brand-gitlab" aria-hidden="true"></i> GitLab CI</span>
      <span class="badge"><i class="ti ti-box" aria-hidden="true"></i> Docker</span>
      <span class="badge">Kubernetes</span>
      <span class="badge">Terraform</span>
      <span class="badge">Ansible</span>
      <span class="badge"><i class="ti ti-terminal" aria-hidden="true"></i> Bash</span>
      <span class="badge">Prometheus</span>
      <span class="badge">Grafana</span>
      <span class="badge">Linux</span>
    </div>
  </div>

  <div id="tab-projects" class="panel">
    <div class="project-card">
      <p class="project-name"><i class="ti ti-git-branch" aria-hidden="true"></i> DevOps Reporting Dashboard</p>
      <p class="project-desc">Full HTML dashboard with login, CRUD, role-based access control, and real-time metrics display.</p>
      <span class="tag">HTML/CSS/JS</span><span class="tag">RBAC</span><span class="tag">Dashboard</span>
    </div>
    <div class="project-card">
      <p class="project-name"><i class="ti ti-box" aria-hidden="true"></i> Inventory Management System</p>
      <p class="project-desc">Web-based inventory system built with modern stack. Designed for enterprise IT asset tracking.</p>
      <span class="tag">Full Stack</span><span class="tag">CRUD</span><span class="tag">REST API</span>
    </div>
    <div class="project-card">
      <p class="project-name"><i class="ti ti-chart-candle" aria-hidden="true"></i> Custom Trading Indicator</p>
      <p class="project-desc">Pine Script indicator for TradingView. Custom signals for technical analysis workflows.</p>
      <span class="tag">Pine Script</span><span class="tag">TradingView</span><span class="tag">TA</span>
    </div>
  </div>

  <div id="tab-stats" class="panel">
    <div class="stat-row">
      <div class="stat-card">
        <div class="stat-num">3+</div>
        <div class="stat-lbl">Active Projects</div>
      </div>
      <div class="stat-card">
        <div class="stat-num">5</div>
        <div class="stat-lbl">DevOps Skills</div>
      </div>
      <div class="stat-card">
        <div class="stat-num">IT→</div>
        <div class="stat-lbl">DevOps Transition</div>
      </div>
      <div class="stat-card">
        <div class="stat-num">MY</div>
        <div class="stat-lbl">Selangor, Malaysia</div>
      </div>
    </div>
    <div class="section-title">Contribution activity (sample)</div>
    <div style="display:flex;gap:3px;flex-wrap:wrap;">
      ${Array.from({length:52}, (_,i) => {
        const h = [0,0,1,2,1,3,2,1,0,1,3,2,1,2,3,1,0,2,3,1,2,0,1,3,2,1,0,2,1,3,2,1,0,1,2,3,1,2,0,1,3,2,1,0,2,1,3,2,1,2,3,1][i] || 0;
        const colors = ['var(--surface-0)','#B5D4F4','#378ADD','#185FA5','#0C447C'];
        return `<div style="width:10px;height:10px;border-radius:2px;background:${colors[h]};"></div>`;
      }).join('')}
    </div>
    <p style="font-size:11px;color:var(--text-muted);margin-top:6px;font-family:var(--font-sans);">Actual data from your GitLab profile</p>
  </div>

  <div id="tab-readme" class="panel">
    <div style="background:var(--surface-1);border:0.5px solid var(--border);border-radius:12px;padding:1rem;">
      <div class="section-title">Raw Markdown — copy into your README.md</div>
      <pre id="readme-content" style="font-size:11px;color:var(--text-secondary);white-space:pre-wrap;overflow-wrap:break-word;line-height:1.6;margin:0;font-family:var(--font-mono);"># Hi, I'm Ijan 👋

**IT Support Engineer → DevOps Engineer**
📍 Selangor, Malaysia | 🏢 Ops.Nexus Data

> Building real pipelines. Automating infrastructure. Shipping reliable systems.

---

## 🛠️ Tech Stack

![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat&logo=gitlab&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat&logo=ansible&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat&logo=linux&logoColor=black)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white)

---

## 🚀 Featured Projects

| Project | Description | Stack |
|---------|-------------|-------|
| 📊 DevOps Dashboard | RBAC reporting dashboard | HTML, CSS, JS |
| 📦 Inventory System | IT asset management app | Full Stack |
| 📈 Trading Indicator | Custom Pine Script signals | Pine Script |

---

## 📊 GitHub/GitLab Stats

![Ijan's Stats](https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=tokyonight)

---

## 📫 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_PROFILE)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:your@email.com)</pre>
      <button class="copy-btn" onclick="copyReadme()"><i class="ti ti-copy" aria-hidden="true"></i> Copy README</button>
    </div>
  </div>
</div>

<script>
function showTab(name) {
  document.querySelectorAll('.panel').forEach(p => p.classList.remove('active'));
  document.querySelectorAll('.tab').forEach(t => { t.classList.remove('active'); t.setAttribute('aria-selected','false'); });
  document.getElementById('tab-' + name).classList.add('active');
  event.target.classList.add('active');
  event.target.setAttribute('aria-selected','true');
}
function copyReadme() {
  const text = document.getElementById('readme-content').textContent;
  navigator.clipboard.writeText(text).then(() => {
    const btn = event.target;
    btn.textContent = '✓ Copied!';
    setTimeout(() => { btn.innerHTML = '<i class="ti ti-copy"></i> Copy README'; }, 2000);
  });
}
</script>
