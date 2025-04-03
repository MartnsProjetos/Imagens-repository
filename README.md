Imagens salvas para implementar no html 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Martins_dev - Currículo</title>
    <style>
        :root {
            --primary-color: #00ff00;
            --background-color: #0a0a14;
            --text-color: #ffffff;
            --section-bg: rgba(30, 30, 50, 0.7);
        }
        
        html {
            box-sizing: border-box;
        }
        
        *, *:before, *:after {
            box-sizing: inherit;
        }
        
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--background-color);
            color: var(--text-color);
            margin: 0;
            padding: 0;
            background-image: linear-gradient(rgba(10, 10, 20, 0.9), rgba(10, 10, 20, 0.9)), url('grid.png');
            background-size: 60px 60px;
            line-height: 1.6;
        }
        
        header {
            text-align: center;
            padding: 2rem 0;
        }
        
        .logo {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 1rem;
        }
        
        .logo span {
            color: var(--primary-color);
        }
        
        nav {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-bottom: 3rem;
        }
        
        nav a {
            color: var(--text-color);
            text-decoration: none;
            font-size: 1.2rem;
            transition: color 0.3s;
        }
        
        nav a:hover {
            color: var(--primary-color);
        }
        
        main {
            max-width: 1000px;
            margin: 0 auto;
            padding: 0 2rem 5rem;
        }
        
        .cv-container {
            background-color: var(--section-bg);
            border-radius: 10px;
            padding: 2rem;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .section-title {
            color: var(--primary-color);
            font-size: 1.8rem;
            margin-bottom: 1rem;
            border-bottom: 1px solid var(--primary-color);
            padding-bottom: 0.5rem;
        }
        
        .cv-section {
            margin-bottom: 2.5rem;
        }
        
        .cv-item {
            margin-bottom: 1.5rem;
        }
        
        .cv-item h3 {
            font-size: 1.3rem;
            margin-bottom: 0.3rem;
        }
        
        .cv-item p {
            margin: 0.3rem 0;
        }
        
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(180px, 1fr));
            gap: 1rem;
        }
        
        .skill-item {
            background: rgba(0, 255, 0, 0.1);
            border: 1px solid rgba(0, 255, 0, 0.3);
            border-radius: 5px;
            padding: 0.5rem 1rem;
            text-align: center;
            transition: all 0.3s;
        }
        
        .skill-item:hover {
            background: rgba(0, 255, 0, 0.2);
            transform: translateY(-3px);
        }
        
        .contact-info {
            display: flex;
            gap: 1.5rem;
            flex-wrap: wrap;
            margin-bottom: 1rem;
        }
        
        .contact-info div {
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .social-icon {
            width: 50px;
            height: 50px;
            background-color: rgba(0, 100, 0, 0.7);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s;
        }
        
        .social-icon:hover {
            background-color: var(--primary-color);
            transform: translateY(-3px);
        }
        
        @media (max-width: 768px) {
            nav {
                flex-direction: column;
                gap: 1rem;
                padding: 0 1rem;
            }
            
            .skills-grid {
                grid-template-columns: 1fr 1fr;
            }
            
            .cv-container {
                padding: 1.5rem;
            }
            
            .contact-info {
                flex-direction: column;
                gap: 0.8rem;
            }
            
            main {
                padding: 0 1rem 3rem;
            }
            
            .section-title {
                font-size: 1.5rem;
            }
            
            .cv-item h3 {
                font-size: 1.2rem;
            }
        }
        
        /* Larger screens */
        @media (min-width: 1200px) {
            .cv-container {
                max-width: 1000px;
                margin: 0 auto;
                padding: 3rem;
            }
            
            .skills-grid {
                grid-template-columns: repeat(4, 1fr);
            }
            
            main {
                max-width: 1200px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">Martins<span>_dev</span></div>
        <nav>
            <a href="index.html">Início</a>
            <a href="curriculo.html">Currículo</a>
            <a href="projetos.html">Projetos</a>
            <a href="sobre.html">Sobre</a>
            <a href="contato.html">Contato</a>
        </nav>
    </header>
    
    <main>
        <div class="cv-container">
            <div class="cv-section">
                <h2 class="section-title">PERFIL PROFISSIONAL</h2>
                <p>Desenvolvedor web full-stack especializado em criação de sites, lojas online e blogs personalizados. Combinando design criativo e performance técnica para transformar ideias em soluções digitais eficientes. Em busca de estágios e oportunidades na área de TI, busco aprendizado de novas tecnologias e contribuição em projetos inovadores. Interessado em aprimorar habilidades em programação, inteligência artificial e análise de dados.</p>
                
                <div class="contact-info">
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>
                        <span>+55 (11) 96382-2159</span>
                    </div>
                    <div>
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
                        <span>mtz.martinss03@gmail.com</span>
                    </div>
                </div>
            </div>
            
            <div class="cv-section">
                <h2 class="section-title">EXPERIÊNCIA PROFISSIONAL</h2>
                
                <div class="cv-item">
                    <h3>FREELANCER</h3>
                    <p>Desenvolvimento de projetos diversos, incluindo freelancers normais e com catálogos de produtos, realizando soluções personalizadas para clientes.</p>
                </div>
                
                <div class="cv-item">
                    <h3>LOJA DE ARTIGOS ESPORTIVOS - @GMBLACKSPORTS</h3>
                    <p>Experiência em gerenciamento de loja, venda de camisas de futebol, criação de anúncios e atendimento a clientes.</p>
                </div>
                
                <div class="cv-item">
                    <h3>OPERADOR DE CARRINHO DE PIPOCA</h3>
                    <p>Atuação com atendimento ao público, prestando um serviço de qualidade e garantindo a satisfação do cliente.</p>
                </div>
                
                <div class="cv-item">
                    <h3>ALUNO MONITOR (GOVERNO)</h3>
                    <p>Auxiliar do professor, ajudando alunos com as lições e facilitando os trabalhos dos professores. (Estágio)</p>
                </div>
            </div>
            
            <div class="cv-section">
                <h2 class="section-title">FORMAÇÃO</h2>
                
                <div class="cv-item">
                    <h3>ENSINO MÉDIO</h3>
                    <p>Cursando no JARDIM ARACATI 2</p>
                    <p>Período NOTURNO - 19H ÀS 23H</p>
                </div>
                
                <div class="cv-item">
                    <h3>ENSINO FUNDAMENTAL</h3>
                    <p>Concluído no EMEF PROF EDVALDO DOS SANTOS DANTAS</p>
                </div>
            </div>
            
            <div class="cv-section">
                <h2 class="section-title">CERTIFICAÇÕES</h2>
                
                <div class="cv-item">
                    <h3>CERTIFICAÇÃO EM INTELIGÊNCIA ARTIFICIAL</h3>
                    <p>Mais IFMG - Curso online</p>
                </div>
                
                <div class="cv-item">
                    <h3>CERTIFICAÇÃO EM JAVASCRIPT (AVANÇADO)</h3>
                    <p>Instituto CEJAM conecta - Presencial</p>
                </div>
                
                <div class="cv-item">
                    <h3>CERTIFICAÇÃO EM PYTHON</h3>
                    <p>Santander - Curso Online</p>
                </div>
                
                <div class="cv-item">
                    <h3>CERTIFICADO DE PACKAGE OFFICE</h3>
                    <p>Excel, PowerPoint e Word - Santander - Curso Online</p>
                </div>
            </div>
            
            <div class="cv-section">
                <h2 class="section-title">PRÊMIOS E CONQUISTAS</h2>
                <div class="cv-item">
                    <p>Medalha de Prata na Olimpíada de Matemática (OBMEP)</p>
                </div>
            </div>
            
            <div class="cv-section">
                <h2 class="section-title">IDIOMAS</h2>
                <div class="cv-item">
                    <p>Português: Nativo</p>
                    <p>Inglês: Básico-Intermediário</p>
                </div>
            </div>
            
            <div class="cv-section">
                <h2 class="section-title">HABILIDADES TÉCNICAS</h2>
                <div class="skills-grid">
                    <div class="skill-item">Desenvolvimento Web</div>
                    <div class="skill-item">Soluções Personalizadas</div>
                    <div class="skill-item">Atendimento ao Público</div>
                    <div class="skill-item">Resolução usando IA</div>
                    <div class="skill-item">Proatividade</div>
                    <div class="skill-item">Design Criativo</div>
                    <div class="skill-item">JavaScript</div>
                    <div class="skill-item">Python</div>
                    <div class="skill-item">Package Office</div>
                </div>
            </div>
            
            <div class="social-links">
                <a href="#" class="social-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg>
                </a>
                <a href="#" class="social-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg>
                </a>
                <a href="#" class="social-icon">
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path><rect x="2" y="9" width="4" height="12"></rect><circle cx="4" cy="4" r="2"></circle></svg>
                </a>
            </div>
        </div>
    </main>
</body>
</html>
