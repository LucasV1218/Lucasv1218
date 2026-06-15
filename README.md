
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:var(--font-sans)}
.screen{padding:2rem 1.5rem;min-height:100vh}
.nav{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:2rem}
.nav-btn{padding:8px 16px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-primary);color:var(--color-text-secondary);cursor:pointer;font-size:13px;font-weight:500;transition:all .15s}
.nav-btn.active{background:#EEEDFE;border-color:#7F77DD;color:#3C3489}
.slide{display:none}
.slide.active{display:block}
h1{font-size:22px;font-weight:500;color:var(--color-text-primary);margin-bottom:4px}
h2{font-size:18px;font-weight:500;color:var(--color-text-primary);margin-bottom:1rem}
h3{font-size:16px;font-weight:500;margin-bottom:.5rem}
.muted{color:var(--color-text-secondary);font-size:14px;margin-bottom:1.5rem}
.card{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1rem 1.25rem;margin-bottom:1rem}
.badge{display:inline-block;padding:3px 10px;border-radius:var(--border-radius-md);font-size:12px;font-weight:500}
.badge-purple{background:#EEEDFE;color:#3C3489}
.badge-teal{background:#E1F5EE;color:#085041}
.badge-amber{background:#FAEEDA;color:#633806}
.badge-coral{background:#FAECE7;color:#712B13}
.badge-blue{background:#E6F1FB;color:#0C447C}
.grid2{display:grid;grid-template-columns:1fr 1fr;gap:1rem;margin-bottom:1rem}
.grid3{display:grid;grid-template-columns:1fr 1fr 1fr;gap:1rem;margin-bottom:1rem}
.code{background:var(--color-background-secondary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-md);padding:.75rem 1rem;font-family:var(--font-mono);font-size:13px;color:var(--color-text-primary);line-height:1.7;margin:.75rem 0}
.kw{color:#534AB7}
.str{color:#0F6E56}
.cm{color:var(--color-text-secondary)}
.vs-row{display:grid;grid-template-columns:1fr 24px 1fr;gap:.5rem;align-items:center;margin-bottom:.5rem}
.vs-label{font-size:13px;padding:6px 10px;border-radius:var(--border-radius-md)}
.vs-left{background:#FAECE7;color:#712B13;text-align:center}
.vs-right{background:#E1F5EE;color:#085041;text-align:center}
.vs-center{text-align:center;font-size:11px;color:var(--color-text-secondary);font-weight:500}
.method-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-top:.75rem}
.method-card{background:var(--color-background-secondary);border-radius:var(--border-radius-md);padding:.6rem .9rem;border-left:3px solid #7F77DD}
.method-name{font-family:var(--font-mono);font-size:13px;font-weight:500;color:#3C3489;margin-bottom:2px}
.method-desc{font-size:12px;color:var(--color-text-secondary)}
.kv-demo{margin:1rem 0}
.kv-row{display:flex;align-items:center;gap:8px;margin-bottom:8px}
.kv-key{background:#EEEDFE;color:#3C3489;padding:6px 14px;border-radius:var(--border-radius-md);font-family:var(--font-mono);font-size:13px;min-width:100px;text-align:center;font-weight:500}
.kv-arrow{color:var(--color-text-secondary);font-size:18px}
.kv-val{background:#E1F5EE;color:#085041;padding:6px 14px;border-radius:var(--border-radius-md);font-family:var(--font-mono);font-size:13px}
.quiz-opt{display:block;width:100%;text-align:left;padding:10px 14px;border:0.5px solid var(--color-border-secondary);border-radius:var(--border-radius-md);background:var(--color-background-primary);color:var(--color-text-primary);cursor:pointer;font-size:14px;margin-bottom:8px;transition:all .15s}
.quiz-opt:hover{background:var(--color-background-secondary)}
.quiz-opt.correct{background:#E1F5EE;border-color:#1D9E75;color:#085041}
.quiz-opt.wrong{background:#FCEBEB;border-color:#E24B4A;color:#791F1F}
.feedback{padding:.75rem 1rem;border-radius:var(--border-radius-md);font-size:14px;margin-top:.5rem;display:none}
.feedback.ok{background:#E1F5EE;color:#085041}
.feedback.err{background:#FCEBEB;color:#791F1F}
.progress{display:flex;gap:6px;margin-bottom:1.5rem}
.progress-dot{width:10px;height:10px;border-radius:50%;background:var(--color-border-tertiary)}
.progress-dot.done{background:#7F77DD}
.progress-dot.current{background:#534AB7}
.section-tag{font-size:11px;font-weight:500;text-transform:uppercase;letter-spacing:.08em;color:var(--color-text-secondary);margin-bottom:.5rem}
.arrow-list li{list-style:none;padding:4px 0;font-size:14px;color:var(--color-text-primary)}
.arrow-list li::before{content:"→ ";color:#7F77DD;font-weight:500}
.big-num{font-size:32px;font-weight:500;color:#534AB7}
.footer-nav{display:flex;justify-content:space-between;margin-top:1.5rem;padding-top:1rem;border-top:0.5px solid var(--color-border-tertiary)}
</style>

<h2 class="sr-only" style="position:absolute;left:-9999px">Revisão interativa de Collections Framework em Java</h2>

<div class="screen">
<div style="display:flex;align-items:center;gap:12px;margin-bottom:.5rem">
  <span class="badge badge-purple">Java</span>
  <span class="badge badge-teal">Collections</span>
  <span class="badge badge-amber">Revisão</span>
</div>
<h1 style="margin-bottom:.25rem">Collections Framework</h1>
<p class="muted">6 objetivos · clique nos tópicos para navegar</p>

<div class="nav" id="nav">
  <button class="nav-btn active" onclick="goTo(0)">1 · O que é</button>
  <button class="nav-btn" onclick="goTo(1)">2 · Array vs ArrayList</button>
  <button class="nav-btn" onclick="goTo(2)">3 · Métodos</button>
  <button class="nav-btn" onclick="goTo(3)">4 · HashMap</button>
  <button class="nav-btn" onclick="goTo(4)">5 · Chave–Valor</button>
  <button class="nav-btn" onclick="goTo(5)">6 · Quiz</button>
</div>

<div class="slide active" id="s0">
  <div class="progress" id="p0">
    <div class="progress-dot current"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
  </div>
  <div class="section-tag">Objetivo 1</div>
  <h2>O que é o Collections Framework?</h2>
  <div class="card">
    <p style="font-size:14px;color:var(--color-text-secondary);margin-bottom:.75rem">Imagine que você tem gavetas em casa. Um Array é uma gaveta com espaços fixos — você decide o tamanho na hora de montar. O <strong>Collections Framework</strong> são gavetas inteligentes: crescem, encolhem e se organizam sozinhas.</p>
    <div class="grid3">
      <div style="background:#EEEDFE;border-radius:var(--border-radius-md);padding:.75rem;text-align:center">
        <div style="font-size:24px;margin-bottom:4px" aria-hidden="true">📦</div>
        <div style="font-size:13px;font-weight:500;color:#3C3489">Listas</div>
        <div style="font-size:12px;color:#534AB7">ArrayList · LinkedList</div>
      </div>
      <div style="background:#E1F5EE;border-radius:var(--border-radius-md);padding:.75rem;text-align:center">
        <div style="font-size:24px;margin-bottom:4px" aria-hidden="true">🗂️</div>
        <div style="font-size:13px;font-weight:500;color:#085041">Mapas</div>
        <div style="font-size:12px;color:#0F6E56">HashMap · TreeMap</div>
      </div>
      <div style="background:#FAEEDA;border-radius:var(--border-radius-md);padding:.75rem;text-align:center">
        <div style="font-size:24px;margin-bottom:4px" aria-hidden="true">🔢</div>
        <div style="font-size:13px;font-weight:500;color:#633806">Sets</div>
        <div style="font-size:12px;color:#854F0B">HashSet · TreeSet</div>
      </div>
    </div>
  </div>
  <div class="card">
    <h3>Por que usar?</h3>
    <ul class="arrow-list">
      <li>Tamanho dinâmico — sem definir antes</li>
      <li>Métodos prontos: busca, ordenação, remoção</li>
      <li>Parte do pacote <span style="font-family:var(--font-mono);font-size:13px;background:var(--color-background-secondary);padding:1px 6px;border-radius:4px">java.util</span></li>
    </ul>
  </div>
  <div class="footer-nav">
    <span></span>
    <button class="nav-btn" onclick="goTo(1)">Próximo →</button>
  </div>
</div>

<div class="slide" id="s1">
  <div class="progress" id="p1">
    <div class="progress-dot done"></div>
    <div class="progress-dot current"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
  </div>
  <div class="section-tag">Objetivo 2</div>
  <h2>Array vs ArrayList</h2>
  <div class="card">
    <div class="vs-row" style="grid-template-columns:80px 1fr 1fr;font-size:12px;font-weight:500;color:var(--color-text-secondary);margin-bottom:.25rem">
      <span></span><span style="text-align:center">Array</span><span style="text-align:center">ArrayList</span>
    </div>
    <div class="vs-row">
      <span style="font-size:12px;color:var(--color-text-secondary)">Tamanho</span>
      <span class="vs-label vs-left">Fixo</span>
      <span class="vs-label vs-right">Dinâmico</span>
    </div>
    <div class="vs-row">
      <span style="font-size:12px;color:var(--color-text-secondary)">Tipos</span>
      <span class="vs-label vs-left">Primitivos</span>
      <span class="vs-label vs-right">Objetos</span>
    </div>
    <div class="vs-row">
      <span style="font-size:12px;color:var(--color-text-secondary)">Sintaxe</span>
      <span class="vs-label vs-left">int[]</span>
      <span class="vs-label vs-right">ArrayList&lt;T&gt;</span>
    </div>
    <div class="vs-row">
      <span style="font-size:12px;color:var(--color-text-secondary)">Métodos</span>
      <span class="vs-label vs-left">Nenhum</span>
      <span class="vs-label vs-right">add, remove…</span>
    </div>
  </div>
  <div class="grid2">
    <div class="card">
      <h3 style="color:#712B13">Array</h3>
      <div class="code"><span class="kw">int</span>[] notas = <span class="kw">new int</span>[3];<br>notas[0] = 8;<br>notas[1] = 7;<br><span class="cm">// tamanho fixo: 3</span></div>
    </div>
    <div class="card">
      <h3 style="color:#085041">ArrayList</h3>
      <div class="code">ArrayList&lt;Integer&gt; notas<br>  = <span class="kw">new</span> ArrayList&lt;&gt;();<br>notas.add(8);<br>notas.add(7); <span class="cm">// sem limite</span></div>
    </div>
  </div>
  <div class="footer-nav">
    <button class="nav-btn" onclick="goTo(0)">← Anterior</button>
    <button class="nav-btn" onclick="goTo(2)">Próximo →</button>
  </div>
</div>

<div class="slide" id="s2">
  <div class="progress" id="p2">
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot current"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
  </div>
  <div class="section-tag">Objetivo 3</div>
  <h2>Métodos do ArrayList</h2>
  <div class="method-grid">
    <div class="method-card">
      <div class="method-name">add(elemento)</div>
      <div class="method-desc">Adiciona ao final da lista</div>
    </div>
    <div class="method-card">
      <div class="method-name">add(índice, elem)</div>
      <div class="method-desc">Insere em posição específica</div>
    </div>
    <div class="method-card">
      <div class="method-name">get(índice)</div>
      <div class="method-desc">Retorna o elemento</div>
    </div>
    <div class="method-card">
      <div class="method-name">remove(índice)</div>
      <div class="method-desc">Remove pelo índice</div>
    </div>
    <div class="method-card">
      <div class="method-name">size()</div>
      <div class="method-desc">Quantidade de elementos</div>
    </div>
    <div class="method-card">
      <div class="method-name">contains(obj)</div>
      <div class="method-desc">Verifica se existe</div>
    </div>
    <div class="method-card">
      <div class="method-name">clear()</div>
      <div class="method-desc">Remove tudo</div>
    </div>
    <div class="method-card">
      <div class="method-name">isEmpty()</div>
      <div class="method-desc">Verifica se está vazia</div>
    </div>
  </div>
  <div class="card">
    <h3>Exemplo completo</h3>
    <div class="code">ArrayList&lt;String&gt; alunos = <span class="kw">new</span> ArrayList&lt;&gt;();<br>alunos.add(<span class="str">"Ana"</span>);<br>alunos.add(<span class="str">"Bruno"</span>);<br>alunos.add(<span class="str">"Carol"</span>);<br>System.out.println(alunos.get(1)); <span class="cm">// Bruno</span><br>System.out.println(alunos.size()); <span class="cm">// 3</span><br>alunos.remove(0); <span class="cm">// remove Ana</span></div>
  </div>
  <div class="footer-nav">
    <button class="nav-btn" onclick="goTo(1)">← Anterior</button>
    <button class="nav-btn" onclick="goTo(3)">Próximo →</button>
  </div>
</div>

<div class="slide" id="s3">
  <div class="progress" id="p3">
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot current"></div>
    <div class="progress-dot"></div>
    <div class="progress-dot"></div>
  </div>
  <div class="section-tag">Objetivo 4</div>
  <h2>HashMap — a estrutura</h2>
  <div class="card">
    <p style="font-size:14px;color:var(--color-text-secondary);margin-bottom:.75rem">Pense no HashMap como um dicionário: você usa uma <strong>palavra (chave)</strong> para encontrar o <strong>significado (valor)</strong>. Acesso direto — sem varrer tudo.</p>
    <div style="display:flex;align-items:center;justify-content:center;gap:1rem;padding:.75rem 0">
      <div style="text-align:center">
        <div class="badge badge-purple" style="display:block;margin-bottom:4px;padding:8px 16px;font-size:13px">Chave</div>
        <div style="font-size:12px;color:var(--color-text-secondary)">qualquer tipo</div>
      </div>
      <div style="font-size:24px;color:var(--color-text-secondary)">→</div>
      <div style="text-align:center">
        <div class="badge badge-teal" style="display:block;margin-bottom:4px;padding:8px 16px;font-size:13px">Valor</div>
        <div style="font-size:12px;color:var(--color-text-secondary)">qualquer tipo</div>
      </div>
    </div>
  </div>
  <div class="card">
    <h3>Criando um HashMap</h3>
    <div class="code">HashMap&lt;String, Integer&gt; notas<br>  = <span class="kw">new</span> HashMap&lt;&gt;();<br><br>notas.put(<span class="str">"Ana"</span>, 9);<br>notas.put(<span class="str">"Bruno"</span>, 7);<br>notas.put(<span class="str">"Carol"</span>, 8);</div>
  </div>
  <div class="card">
    <h3>Principais métodos</h3>
    <div class="method-grid">
      <div class="method-card" style="border-left-color:#1D9E75">
        <div class="method-name" style="color:#085041">put(chave, valor)</div>
        <div class="method-desc">Insere ou atualiza</div>
      </div>
      <div class="method-card" style="border-left-color:#1D9E75">
        <div class="method-name" style="color:#085041">get(chave)</div>
        <div class="method-desc">Retorna o valor</div>
      </div>
      <div class="method-card" style="border-left-color:#1D9E75">
        <div class="method-name" style="color:#085041">containsKey(c)</div>
        <div class="method-desc">A chave existe?</div>
      </div>
      <div class="method-card" style="border-left-color:#1D9E75">
        <div class="method-name" style="color:#085041">remove(chave)</div>
        <div class="method-desc">Remove o par</div>
      </div>
    </div>
  </div>
  <div class="footer-nav">
    <button class="nav-btn" onclick="goTo(2)">← Anterior</button>
    <button class="nav-btn" onclick="goTo(4)">Próximo →</button>
  </div>
</div>

<div class="slide" id="s4">
  <div class="progress" id="p4">
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot current"></div>
    <div class="progress-dot"></div>
  </div>
  <div class="section-tag">Objetivo 5 · 6</div>
  <h2>Chave–Valor na prática</h2>
  <div class="card">
    <p class="muted" style="margin-bottom:.75rem">Exemplo: cadastro de alunos por CPF</p>
    <div class="kv-demo">
      <div class="kv-row">
        <span class="kv-key">"123.456"</span>
        <span class="kv-arrow">→</span>
        <span class="kv-val">"Ana Paula"</span>
      </div>
      <div class="kv-row">
        <span class="kv-key">"789.012"</span>
        <span class="kv-arrow">→</span>
        <span class="kv-val">"Bruno Lima"</span>
      </div>
      <div class="kv-row">
        <span class="kv-key">"345.678"</span>
        <span class="kv-arrow">→</span>
        <span class="kv-val">"Carol Souza"</span>
      </div>
    </div>
    <div class="code">HashMap&lt;String, String&gt; cadastro<br>  = <span class="kw">new</span> HashMap&lt;&gt;();<br><br>cadastro.put(<span class="str">"123.456"</span>, <span class="str">"Ana Paula"</span>);<br><br><span class="cm">// Recuperar:</span><br>String nome = cadastro.get(<span class="str">"123.456"</span>);<br>System.out.println(nome); <span class="cm">// Ana Paula</span><br><br><span class="cm">// Percorrer tudo:</span><br><span class="kw">for</span> (String cpf : cadastro.keySet()) {<br>  System.out.println(cpf + <span class="str">" → "</span><br>    + cadastro.get(cpf));<br>}</div>
  </div>
  <div class="footer-nav">
    <button class="nav-btn" onclick="goTo(3)">← Anterior</button>
    <button class="nav-btn" onclick="goTo(5)">Quiz final →</button>
  </div>
</div>

<div class="slide" id="s5">
  <div class="progress" id="p5">
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot done"></div>
    <div class="progress-dot current"></div>
  </div>
  <div class="section-tag">Quiz</div>
  <h2>Teste seus conhecimentos</h2>

  <div id="q0" class="card">
    <h3 style="margin-bottom:.75rem">1. Qual é a diferença principal entre Array e ArrayList?</h3>
    <button class="quiz-opt" onclick="ans(0,0)">a) Array usa objetos, ArrayList usa primitivos</button>
    <button class="quiz-opt" onclick="ans(0,1)">b) Array tem tamanho fixo, ArrayList é dinâmico</button>
    <button class="quiz-opt" onclick="ans(0,2)">c) Não há diferença prática</button>
    <button class="quiz-opt" onclick="ans(0,3)">d) ArrayList pertence ao pacote java.lang</button>
    <div class="feedback" id="f0"></div>
  </div>

  <div id="q1" class="card">
    <h3 style="margin-bottom:.75rem">2. Qual método adiciona um elemento no ArrayList?</h3>
    <button class="quiz-opt" onclick="ans(1,0)">a) insert()</button>
    <button class="quiz-opt" onclick="ans(1,1)">b) push()</button>
    <button class="quiz-opt" onclick="ans(1,2)">c) add()</button>
    <button class="quiz-opt" onclick="ans(1,3)">d) append()</button>
    <div class="feedback" id="f1"></div>
  </div>

  <div id="q2" class="card">
    <h3 style="margin-bottom:.75rem">3. No HashMap, o que é a "chave"?</h3>
    <button class="quiz-opt" onclick="ans(2,0)">a) Um índice numérico como no Array</button>
    <button class="quiz-opt" onclick="ans(2,1)">b) O identificador único para acessar o valor</button>
    <button class="quiz-opt" onclick="ans(2,2)">c) Sempre uma String obrigatoriamente</button>
    <button class="quiz-opt" onclick="ans(2,3)">d) O nome do objeto armazenado</button>
    <div class="feedback" id="f2"></div>
  </div>

  <div id="score-area" style="display:none;margin-top:1rem">
    <div class="card" style="text-align:center;padding:1.5rem">
      <div class="big-num" id="score-num">0/3</div>
      <p style="color:var(--color-text-secondary);font-size:14px;margin-top:.5rem" id="score-msg"></p>
      <div style="margin-top:1rem;display:flex;gap:8px;justify-content:center;flex-wrap:wrap">
        <button class="nav-btn" onclick="goTo(0)" style="font-size:13px">Revisar tudo</button>
        <button class="nav-btn" onclick="sendPrompt('Me dê um exercício de codificação usando ArrayList e HashMap juntos')" style="font-size:13px">Exercício prático ↗</button>
      </div>
    </div>
  </div>
</div>

</div>

<script>
var cur=0;
var answers=[1,2,1];
var correct=[false,false,false];
var answered=[false,false,false];
var msgs=["Revise os tópicos antes de continuar. Você consegue!","Bom trabalho! Pratique mais um pouco.","Perfeito! Partiu código!"];

function goTo(n){
  document.querySelectorAll('.slide').forEach(function(s){s.classList.remove('active')});
  document.querySelectorAll('.nav-btn').forEach(function(b,i){b.classList.toggle('active',i===n)});
  document.getElementById('s'+n).classList.add('active');
  cur=n;
}

function ans(q,choice){
  if(answered[q])return;
  answered[q]=true;
  var opts=document.querySelectorAll('#q'+q+' .quiz-opt');
  var fb=document.getElementById('f'+q);
  opts.forEach(function(o){o.disabled=true});
  if(choice===answers[q]){
    opts[choice].classList.add('correct');
    correct[q]=true;
    fb.textContent='Correto! '+getFeedback(q,true);
    fb.className='feedback ok';
  } else {
    opts[choice].classList.add('wrong');
    opts[answers[q]].classList.add('correct');
    fb.textContent='Não era essa. '+getFeedback(q,false);
    fb.className='feedback err';
  }
  fb.style.display='block';
  var total=correct.filter(Boolean).length;
  if(answered.every(Boolean)){
    var sa=document.getElementById('score-area');
    sa.style.display='block';
    document.getElementById('score-num').textContent=total+'/3';
    document.getElementById('score-msg').textContent=msgs[total];
  }
}

function getFeedback(q,ok){
  var tips=[
    ok?'Array é gaveta fixa, ArrayList é elástica.':'Lembre: quem é fixo é o Array.',
    ok?'add() é o método padrão para inserir.':'push() é JavaScript. Em Java é add().',
    ok?'A chave pode ser String, Integer, qualquer objeto.':'Chave é o identificador — pode ser qualquer tipo.'
  ];
  return tips[q];
}
</script>
