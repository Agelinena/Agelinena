<div align="center">

<img src="banner.svg" alt="Agelinena, alienígena de cibersegurança" width="100%"/>

<a href="https://github.com/Agelinena">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3200&pause=900&color=7FF5C4&center=true&vCenter=true&width=720&lines=Olá%2C+terráqueo!+Eu+sou+o+Lucas+%F0%9F%91%BD;Blue+Team+%2F+SOC+em+formação+%F0%9F%9B%A1%EF%B8%8F;Detectar%2C+conter%2C+endurecer+%F0%9F%94%90;Homelab+self-hosted+sempre+no+ar+%F0%9F%96%A5%EF%B8%8F" alt="Frases animadas"/>
</a>

<br/>

![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-005571?style=for-the-badge)
![CrowdStrike](https://img.shields.io/badge/CrowdStrike-EDR-FC0000?style=for-the-badge&logo=crowdstrike&logoColor=white)
![OPNsense](https://img.shields.io/badge/OPNsense-Firewall-D94F00?style=for-the-badge&logo=opnsense&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-Hardening-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-Automação-3776AB?style=for-the-badge&logo=python&logoColor=white)

</div>

---

## 👋 Olá, eu sou o Lucas Lindemann Anschau do Amaral

🛸 Por aqui me chamam de **Agelinena** (*alienígena*), meu usuário em tudo.

🎓 Estudante de **Tecnologia em Segurança Cibernética** no **Senac RS** (conclusão prevista: 2029)

🛡️ **Estagiário de Segurança da Informação na AESC**: triagem de incidentes no CrowdStrike, segurança de e-mail com Trend AI, chamados de TI, relatórios gerenciais e palestras de conscientização

🏠 Mantenho um **homelab self-hosted** com foco em hardening e monitoramento contínuo

🎯 Buscando atuar em **Blue Team / SOC**, unindo análise de incidentes e automação

---

## 🧰 Tecnologias e ferramentas

| 🛡️ Segurança | 🌐 Infra e redes | 🐍 Automação | 🧪 Práticas |
|:--|:--|:--|:--|
| Wazuh (FIM, SCA, correlação) | Docker | Python (scripts, OOP) | Hardening de sistemas |
| OPNsense (Firewall, VLAN, DoT) | Linux | SQL (MySQL) | Segmentação de rede |
| CrowdStrike (EDR) | Traefik (proxy reverso, TLS) | n8n | Pentest web (OWASP) |
| Trend AI (e-mail) | Tailscale (VPN) | APIs e Webhooks | Gestão de chamados de TI |
| Authentik (SSO) e Vaultwarden | Git | | |

---

## 🗺️ Mapa do meu homelab

Diagrama interativo, com zoom e arraste no GitHub. Ajuste os nós conforme sua topologia real.

```mermaid
flowchart LR
    NET((Internet)) --> FW["OPNsense<br/>Firewall, DoT/Quad9, AdGuard"]
    TS["Tailscale<br/>subnet router / exit node"] --- FW
    FW --> V1["VLAN de serviços<br/>egresso restrito"]
    FW --> V2["VLAN de gestão"]
    V1 --> PX["Traefik<br/>TLS wildcard via DNS-01"]
    PX --> AK["Authentik<br/>SSO + ForwardAuth"]
    AK --> APPS["Serviços self-hosted"]
    VW["Vaultwarden<br/>senhas e segredos"] -.-> APPS
    WZ["Wazuh<br/>logs, FIM, SCA, rootkits"] -. monitora .-> APPS
    WZ -. monitora .-> FW

    classDef sec fill:#0b1030,stroke:#7ff5c4,color:#eafff6;
    class FW,AK,WZ,VW,PX sec;
```

---

## 📂 Projetos em destaque

<details>
<summary><b>🔥 Firewall e VPN (OPNsense)</b></summary>
<br/>

Regras de firewall, filtragem DNS com DoT/Quad9 e AdGuard, bloqueio anti-bypass e acesso remoto seguro via Tailscale (subnet router e exit node).

</details>

<details>
<summary><b>🧱 Segmentação de rede</b></summary>
<br/>

Isolamento de tráfego em VLANs e redes internas por serviço, com políticas de egresso restritas e defesa em profundidade.

</details>

<details>
<summary><b>🔒 Proxy e TLS (Traefik)</b></summary>
<br/>

Reverse proxy centralizado com certificados TLS wildcard automatizados (Let's Encrypt via DNS-01) e exposição seletiva de serviços.

</details>

<details>
<summary><b>🪪 IAM e segredos (Authentik + Vaultwarden)</b></summary>
<br/>

SSO/IdP com ForwardAuth para proteger painéis administrativos e gerenciamento de senhas e segredos fora do versionamento.

</details>

<details>
<summary><b>📡 SIEM e monitoramento (Wazuh)</b></summary>
<br/>

Agente para coleta de logs, correlação de eventos, monitoramento de integridade de arquivos (FIM), detecção de rootkits e avaliação de hardening (SCA).

</details>

<details>
<summary><b>🛸 Easter egg</b></summary>
<br/>

Você achou o esconderijo do alienígena. Se quiser trocar ideia sobre SOC, homelab ou Blue Team, é só chamar.

</details>

---

## 📜 Certificações

- 🛡️ **Segurança de redes: firewall, WAF e SIEM**, Alura
- 🕷️ **Pentest: explorando vulnerabilidades em aplicações web**, Alura
- 💀 **Fundamental Hacking (60h)**, HackerSec

---

## 📊 Atividade no GitHub

<div align="center">

<img height="170" src="https://github-readme-stats.vercel.app/api?username=Agelinena&show_icons=true&hide_border=true&bg_color=0b1030&title_color=7ff5c4&icon_color=ffb454&text_color=eafff6" alt="Estatísticas do GitHub"/>
<img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Agelinena&layout=compact&hide_border=true&bg_color=0b1030&title_color=7ff5c4&text_color=eafff6" alt="Linguagens mais usadas"/>

<img src="https://streak-stats.demolab.com?user=Agelinena&hide_border=true&background=0b1030&ring=7ff5c4&fire=ffb454&currStreakLabel=7ff5c4&sideLabels=b9b4ff&currStreakNum=eafff6&sideNums=eafff6&dates=b9b4ff" alt="Sequência de contribuições"/>

</div>

---

## 📫 Como me encontrar

<div align="center">

[![Email](https://img.shields.io/badge/Email-lucaslamaral%40proton.me-6D4AFF?style=for-the-badge&logo=protonmail&logoColor=white)](mailto:lucaslamaral@proton.me)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Lucas%20Amaral-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucaslindemann)
[![GitHub](https://img.shields.io/badge/GitHub-Agelinena-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Agelinena)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:070b1f,50:2b3a8f,100:7ff5c4&height=110&section=footer" width="100%" alt=""/>

</div>
