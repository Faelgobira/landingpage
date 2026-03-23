<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MJ Consultoria Imobiliária | High-End Rio</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700&family=Inter:wght@300;400&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #C5A059;
            --black: #1A1A1A;
            --white: #F5F5F7;
            --text: #333;
        }

        * { margin: 0; padding: 0; box-sizing: border-box; }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--white);
            color: var(--text);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Header */
        header {
            padding: 30px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: absolute;
            width: 100%;
            z-index: 10;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 24px;
            letter-spacing: 4px;
            color: var(--black);
            font-weight: 700;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 10%;
            background: linear-gradient(rgba(245,245,247,0.8), rgba(245,245,247,0.8)), url('https://images.unsplash.com/photo-1483729558449-99ef09a8c325?auto=format&fit=crop&q=80&w=2070') no-repeat center center/cover;
        }

        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: clamp(2.5rem, 5vw, 4rem);
            margin-bottom: 20px;
            font-weight: 400;
        }

        .hero p {
            max-width: 600px;
            font-size: 1.1rem;
            color: #666;
            margin-bottom: 40px;
        }

        .btn-primary {
            padding: 18px 40px;
            background: var(--black);
            color: white;
            text-decoration: none;
            letter-spacing: 2px;
            font-size: 13px;
            transition: 0.3s;
        }

        .btn-primary:hover { background: var(--gold); }

        /* Portfolio Grid */
        .portfolio { padding: 100px 5%; }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 40px;
        }

        .card { position: relative; overflow: hidden; background: #fff; }
        .card img {
            width: 100%;
            height: 500px;
            object-fit: cover;
            filter: grayscale(20%);
            transition: 0.5s;
        }
        .card:hover img { transform: scale(1.05); filter: grayscale(0%); }
        .card-info { padding: 20px 0; }
        .card-info h3 { font-family: 'Playfair Display', serif; font-size: 1.5rem; }
        .card-info p { color: var(--gold); font-size: 0.9rem; text-transform: uppercase; letter-spacing: 1px; }

        /* Form Section */
        .contact {
            padding: 100px 5%;
            background: var(--black);
            color: white;
            text-align: center;
        }

        .contact h2 { font-family: 'Playfair Display', serif; font-size: 2.5rem; margin-bottom: 50px; }

        form {
            max-width: 500px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        input {
            padding: 15px;
            background: transparent;
            border: none;
            border-bottom: 1px solid #444;
            color: white;
            font-family: inherit;
        }

        input:focus { outline: none; border-bottom-color: var(--gold); }

        .submit-btn {
            margin-top: 20px;
            padding: 20px;
            background: var(--white);
            color: var(--black);
            border: none;
            cursor: pointer;
            font-weight: bold;
            letter-spacing: 2px;
        }

        footer { padding: 50px; text-align: center; font-size: 12px; color: #999; }

        @media (max-width: 768px) {
            .hero h1 { font-size: 2.2rem; }
            .grid { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">MJ</div>
        <div style="font-size: 12px; letter-spacing: 1px;">RIO DE JANEIRO</div>
    </header>

    <section class="hero">
        <p>COLEÇÃO PRIVADA 2026</p>
        <h1>A arte de viver o extraordinário no Rio.</h1>
        <p>Curadoria seleta de propriedades de alto padrão e unidades off-market nas localizações mais cobiçadas da cidade.</p>
        <a href="#contato" class="btn-primary">EXPLORAR PORTFÓLIO</a>
    </section>

    <section class="portfolio">
        <div class="grid">
            <div class="card">
                <img src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?auto=format&fit=crop&q=80&w=2070" alt="Ipanema">
                <div class="card-info">
                    <p>Ipanema</p>
                    <h3>The Penthouse Legacy</h3>
                </div>
            </div>
            <div class="card">
                <img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&q=80&w=2070" alt="Joá">
                <div class="card-info">
                    <p>Joá</p>
                    <h3>Residência Aurora</h3>
                </div>
            </div>
            <div class="card">
                <img src="https://images.unsplash.com/photo-1600607687940-4e2003e25489?auto=format&fit=crop&q=80&w=2070" alt="Leblon">
                <div class="card-info">
                    <p>Leblon</p>
                    <h3>Edifício Vanguarda</h3>
                </div>
            </div>
        </div>
    </section>

    <section class="contact" id="contato">
        <h2>Inicie sua jornada exclusiva</h2>
        <form>
            <input type="text" placeholder="Nome Completo">
            <input type="email" placeholder="E-mail Pessoal">
            <input type="tel" placeholder="WhatsApp">
            <button type="submit" class="submit-btn">SOLICITAR CONSULTORIA PRIVADA</button>
        </form>
    </section>

    <footer>
        <p>© 2026 MJ CONSULTORIA IMOBILIÁRIA - TODOS OS DIREITOS RESERVADOS</p>
    </footer>

</body>
</html>
