<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>COGIC - Igreja de Deus em Cristo</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f8f9fa;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #2c3e50 0%, #3498db 100%);
            color: white;
            padding: 1rem 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: bold;
            text-decoration: none;
            color: white;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        nav a:hover, nav a.active {
            background-color: rgba(255,255,255,0.2);
        }

        /* Main Content */
        main {
            padding: 2rem 0;
        }

        .page {
            display: none;
            animation: fadeIn 0.5s ease-in;
        }

        .page.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(44, 62, 80, 0.8), rgba(52, 152, 219, 0.8)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%23e3f2fd" width="1200" height="600"/><path fill="%23bbdefb" d="M600,50 L700,200 L500,200 Z"/><circle fill="%2390caf9" cx="300" cy="400" r="80"/><circle fill="%2364b5f6" cx="900" cy="350" r="60"/></svg>');
            color: white;
            text-align: center;
            padding: 4rem 0;
            border-radius: 10px;
            margin-bottom: 2rem;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .cta-button {
            background-color: #e74c3c;
            color: white;
            padding: 1rem 2rem;
            text-decoration: none;
            border-radius: 50px;
            font-weight: bold;
            display: inline-block;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 5px 15px rgba(231, 76, 60, 0.4);
        }

        /* Cards */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }

        .card {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .card h3 {
            color: #2c3e50;
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }

        .card p {
            color: #666;
            margin-bottom: 1rem;
        }

        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 3rem;
            margin: 2rem 0;
            align-items: center;
        }

        .about-text h2 {
            color: #2c3e50;
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .about-text p {
            color: #666;
            margin-bottom: 1.5rem;
            font-size: 1.1rem;
        }

        .about-image {
            background: linear-gradient(45deg, #3498db, #2c3e50);
            height: 300px;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.2rem;
            text-align: center;
        }

        /* Contact Form */
        .contact-form {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            max-width: 600px;
            margin: 2rem auto;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            color: #2c3e50;
            font-weight: bold;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 0.8rem;
            border: 2px solid #e9ecef;
            border-radius: 5px;
            font-size: 1rem;
            transition: border-color 0.3s ease;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #3498db;
        }

        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }

        .submit-btn {
            background-color: #3498db;
            color: white;
            padding: 1rem 2rem;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s ease;
            width: 100%;
        }

        .submit-btn:hover {
            background-color: #2980b9;
        }

        /* Footer */
        footer {
            background-color: #2c3e50;
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 3rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h3 {
            margin-bottom: 1rem;
            color: #3498db;
        }

        .footer-section p, .footer-section a {
            color: #bdc3c7;
            text-decoration: none;
        }

        .footer-section a:hover {
            color: white;
        }

        /* Bible Verse */
        .bible-verse {
            background: linear-gradient(45deg, #f39c12, #e67e22);
            color: white;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            margin: 2rem 0;
            font-style: italic;
        }

        .bible-verse p {
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }

        .bible-verse cite {
            font-weight: bold;
            font-size: 1.1rem;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                gap: 1rem;
            }

            nav ul {
                flex-direction: column;
                gap: 1rem;
            }

            .hero h1 {
                font-size: 2rem;
            }

            .about-content {
                grid-template-columns: 1fr;
            }

            .cards-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <a href="#" class="logo">COGIC</a>
                <nav>
                    <ul>
                        <li><a href="#" class="nav-link active" data-page="home">Início</a></li>
                        <li><a href="#" class="nav-link" data-page="about">Sobre Nós</a></li>
                        <li><a href="#" class="nav-link" data-page="contact">Contato</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <main class="container">
        <!-- Página Inicial -->
        <div id="home" class="page active">
            <section class="hero">
                <h1>Igreja de Deus em Cristo</h1>
                <p>Bem-vindos à nossa congregação! Somos uma comunidade de fé unida pelo amor de Cristo, dedicada ao culto, comunhão e serviço ao próximo.</p>
                <a href="#" class="cta-button">Venha nos Conhecer</a>
            </section>

            <div class="bible-verse">
                <p>"E perseveravam na doutrina dos apóstolos, e na comunhão, e no partir do pão, e nas orações."</p>
                <cite>Atos 2:42</cite>
            </div>

            <section class="cards-grid">
                <div class="card">
                    <h3>🙏 Cultos</h3>
                    <p>Participe dos nossos cultos de adoração, onde experimentamos a presença de Deus através de louvores, orações e pregação da Palavra.</p>
                </div>
                <div class="card">
                    <h3>📖 Escola Bíblica</h3>
                    <p>Aprofunde-se no conhecimento das Escrituras através de estudos bíblicos sistemáticos e classes para todas as idades.</p>
                </div>
                <div class="card">
                    <h3>👨‍👩‍👧‍👦 Ministérios</h3>
                    <p>Temos ministérios para crianças, jovens, adultos e idosos, cada um com atividades específicas para edificação espiritual.</p>
                </div>
                <div class="card">
                    <h3>🤝 Comunhão</h3>
                    <p>Vivemos em comunhão cristã, compartilhando alegrias, tristezas e apoiando uns aos outros em oração e amor fraternal.</p>
                </div>
                <div class="card">
                    <h3>💒 Eventos</h3>
                    <p>Participamos de conferências, congressos, retiros espirituais e eventos especiais que fortalecem nossa fé e união.</p>
                </div>
                <div class="card">
                    <h3>🌍 Missões</h3>
                    <p>Levamos o evangelho além dos muros da igreja através de trabalhos missionários e evangelismo na comunidade.</p>
                </div>
            </section>
        </div>

        <!-- Página Sobre -->
        <div id="about" class="page">
            <section class="about-content">
                <div class="about-text">
                    <h2>Nossa História</h2>
                    <p>A Igreja de Deus em Cristo (COGIC) foi fundada com o propósito de adorar a Deus em espírito e verdade, seguindo os ensinamentos de Jesus Cristo e a doutrina apostólica.</p>
                    <p>Somos uma congregação que busca viver os princípios bíblicos em nossa jornada de fé, crescendo juntos em santidade e amor cristão.</p>
                    <p>Nossa comunidade é formada por irmãos e irmãs unidos pela graça de Deus, comprometidos com a oração, o estudo da Palavra e o testemunho cristão.</p>
                </div>
                <div class="about-image">
                    <div>
                        <h3>Nossa Missão</h3>
                        <p>Adorar a Deus, edificar os santos e evangelizar o mundo através do poder do Espírito Santo</p>
                    </div>
                </div>
            </section>

            <div class="bible-verse">
                <p>"Ide, portanto, fazei discípulos de todas as nações, batizando-os em nome do Pai, e do Filho, e do Espírito Santo."</p>
                <cite>Mateus 28:19</cite>
            </div>

            <section class="cards-grid">
                <div class="card">
                    <h3>🎯 Nosso Propósito</h3>
                    <p>Glorificar a Deus através da adoração, crescer em santidade, edificar o corpo de Cristo e levar o evangelho a toda criatura.</p>
                </div>
                <div class="card">
                    <h3>✝️ Nossa Doutrina</h3>
                    <p>Fundamentamos nossa fé nas Sagradas Escrituras, na salvação pela graça, no batismo em águas e na santificação progressiva.</p>
                </div>
                <div class="card">
                    <h3>🕊️ Nossos Valores</h3>
                    <p>Amor fraternal, santidade, oração, estudo da Palavra, comunhão, evangelismo e serviço cristão em nossa comunidade.</p>
                </div>
            </section>
        </div>

        <!-- Página Contato -->
        <div id="contact" class="page">
            <section>
                <h2 style="text-align: center; color: #2c3e50; margin-bottom: 2rem; font-size: 2.5rem;">Fale Conosco</h2>
                <p style="text-align: center; color: #666; margin-bottom: 3rem; font-size: 1.1rem;">Queremos conhecê-lo! Entre em contato conosco para mais informações sobre nossa congregação.</p>
                
                <form class="contact-form" onsubmit="handleSubmit(event)">
                    <div class="form-group">
                        <label for="name">Nome Completo</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="email">E-mail</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="phone">Telefone</label>
                        <input type="tel" id="phone" name="phone">
                    </div>
                    
                    <div class="form-group">
                        <label for="subject">Assunto</label>
                        <select id="subject" name="subject" style="width: 100%; padding: 0.8rem; border: 2px solid #e9ecef; border-radius: 5px; font-size: 1rem;">
                            <option value="">Selecione um assunto</option>
                            <option value="visita">Quero visitar a igreja</option>
                            <option value="oracao">Pedido de oração</option>
                            <option value="batismo">Informações sobre batismo</option>
                            <option value="ministerio">Interesse em ministério</option>
                            <option value="evento">Informações sobre eventos</option>
                            <option value="outro">Outro</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="message">Mensagem</label>
                        <textarea id="message" name="message" required placeholder="Conte-nos como podemos ajudá-lo em sua jornada de fé..."></textarea>
                    </div>
                    
                    <button type="submit" class="submit-btn">Enviar Mensagem</button>
                </form>
            </section>

            <section class="cards-grid" style="margin-top: 3rem;">
                <div class="card">
                    <h3>📧 E-mail</h3>
                    <p>contato@cogic.com.br<br>
                       pastor@cogic.com.br<br>
                       secretaria@cogic.com.br</p>
                </div>
                <div class="card">
                    <h3>📱 Telefone</h3>
                    <p>(11) 3456-7890<br>
                       (11) 9 8765-4321<br>
                       <em>Seg a Sex: 9h às 18h</em></p>
                </div>
                <div class="card">
                    <h3>📍 Endereço</h3>
                    <p>Rua da Congregação, 123<br>
                       Bairro da Paz<br>
                       São Paulo - SP<br>
                       CEP: 01234-567</p>
                </div>
            </section>

            <div class="bible-verse">
                <p>"Invoca-me no dia da angústia; eu te livrarei, e tu me glorificarás."</p>
                <cite>Salmos 50:15</cite>
            </div>
        </div>
    </main>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>COGIC</h3>
                    <p>Igreja de Deus em Cristo - Uma comunidade de fé, adoração e serviço ao Senhor Jesus.</p>
                </div>
                <div class="footer-section">
                    <h3>Horários de Culto</h3>
                    <p>Domingo: 9h e 19h</p>
                    <p>Quarta: 19h30</p>
                    <p>Sexta: 19h30</p>
                    <p>Sábado: 19h (Jovens)</p>
                </div>
                <div class="footer-section">
                    <h3>Redes Sociais</h3>
                    <p><a href="#">Facebook</a></p>
                    <p><a href="#">Instagram</a></p>
                    <p><a href="#">YouTube</a></p>
                    <p><a href="#">WhatsApp</a></p>
                </div>
            </div>
            <p>&copy; 2025 Igreja de Deus em Cristo (COGIC). Todos os direitos reservados.</p>
        </div>
    </footer>

    <script>
        // Navegação entre páginas
        document.addEventListener('DOMContentLoaded', function() {
            const navLinks = document.querySelectorAll('.nav-link');
            const pages = document.querySelectorAll('.page');

            navLinks.forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    
                    // Remove active class from all links and pages
                    navLinks.forEach(l => l.classList.remove('active'));
                    pages.forEach(p => p.classList.remove('active'));
                    
                    // Add active class to clicked link
                    this.classList.add('active');
                    
                    // Show corresponding page
                    const targetPage = this.getAttribute('data-page');
                    document.getElementById(targetPage).classList.add('active');
                });
            });
        });

        // Função para lidar com o envio do formulário
        function handleSubmit(event) {
            event.preventDefault();
            
            const form = event.target;
            const formData = new FormData(form);
            
            // Simular envio (aqui você integraria com um serviço real)
            const submitBtn = form.querySelector('.submit-btn');
            const originalText = submitBtn.textContent;
            
            submitBtn.textContent = 'Enviando...';
            submitBtn.disabled = true;
            
            setTimeout(() => {
                alert('Mensagem enviada com sucesso! Entraremos em contato em breve. Deus te abençoe!');
                form.reset();
                submitBtn.textContent = originalText;
                submitBtn.disabled = false;
            }, 2000);
        }

        // Animação smooth nos botões CTA
        document.querySelectorAll('.cta-button').forEach(button => {
            button.addEventListener('click', function(e) {
                e.preventDefault();
                
                // Navegar para a página de contato
                document.querySelectorAll('.nav-link').forEach(l => l.classList.remove('active'));
                document.querySelectorAll('.page').forEach(p => p.classList.remove('active'));
                
                document.querySelector('[data-page="contact"]').classList.add('active');
                document.getElementById('contact').classList.add('active');
            });
        });
    </script>
</body>
</html>
