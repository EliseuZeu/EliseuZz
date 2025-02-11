<div align="center">
  <h3>👋 Olá, eu sou o EliseuZz</h3>
  
  <p>🐺 Me chamo Eliseu Francisco de Souza</p>
  <p>🧔 Eu estudo Análise e Desenvolvimento de Sistemas na Universidade São Francisco</p>
  <p>🧠 Sou um entusiasta de tecnologia e programação</p>

  <br/>

  <img width="600" alt="Skills / cool things" src="https://skills-icons.vercel.app/api/icons?i=python,java,html,css,js,github,git,vscode,linux,node,react,firebase,tailwind&perline=14" />
</div>

<hr />

{% if followers|length > 0 %}
<div align="center">
    <h4>👤 Seguidores 👤</h4>
    <p><i>Quer fazer parte? Só me seguir!</i></p>
    <img width="600" src=".github/assets/cards/top3.svg" alt="Top 3 seguidores mais ativos" />
    {% if followers|length > 2 and total_contributions > 0 %}
    <details>
    <summary>🏅 Classificações 🏅</summary>
    <br/>
    <table>
        <thead>
            <tr align="center">
                <th>Posição</th>
                <th>Seguidor</th>
                <th>Contribuições</th>
            </tr>
        </thead>
        <tbody>
            {% for position, name, url, contributions in followers %}
            {% if contributions > 0 %}
            <tr align="center">
                <td>{{ position + 1 }}°</td>
                <td><a href="{{ url }}">{{ name }}</a></td>
                <td>{{ contributions }} ctr.</td>
            </tr>
            {% endif %}
            {% endfor %}
        </tbody>
    </table>
    </details>
    <details>
    <summary>✨ Review da IA ✨</summary>
    <br/>
    <div align="justify">{{ ai_review }}</div>
    </details>
    {% endif %}
</div>
{% endif %}

<div align="center">
  <h4>🐍 Snakommits 🐍</h4>
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/EliseuZeu/EliseuZeu/snake-output/snake-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/EliseuZeu/EliseuZeu/snake-output/snake-light.svg">
      <img alt="github contribution grid snake animation" src="https://raw.githubusercontent.com/EliseuZeu/EliseuZeu/snake-output/snake-light.svg">
    </picture>
</div>

<h6 align="right">
  Esse perfil é atualizado diariamente!<br/> <i>{{ last_update }}</i>
<h6>