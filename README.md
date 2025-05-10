 Nk
 <!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CADU NK - Artista de Eletro Funk</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
    <script src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
    <script src="https://unpkg.com/babel-standalone@6/babel.min.js"></script>
    <style>
        body {
            background: linear-gradient(135deg, #1a1a1a, #2c003e);
            color: #ffffff;
            font-family: 'Arial', sans-serif;
        }
        .glow-text {
            text-shadow: 0 0 10px #ff00ff, 0 0 20px #00ffcc;
        }
        .neon-border {
            box-shadow: 0 0 10px #ff00ff, 0 0 20px #00ffcc;
        }
        .gallery-img {
            transition: transform 0.3s ease;
        }
        .gallery-img:hover {
            transform: scale(1.05);
        }
    </style>
</head>
<body>
    <div id="root"></div>

    <script type="text/babel">
        function Header() {
            return (
                <header className="py-6 text-center">
                    <h1 className="text-5xl font-bold glow-text">CADU NK</h1>
                    <p className="text-xl mt-2">O Som que Agita Goiânia</p>
                </header>
            );
        }

        function Bio() {
            return (
                <section className="max-w-4xl mx-auto p-6 text-center">
                    <h2 className="text-3xl font-bold mb-4 glow-text">Sobre Mim</h2>
                    <p className="text-lg">
                        Eu sou CADU NK, artista de eletro funk com 20 anos, trazendo o grave que faz tremer desde os 14. Com hits como 
                        <span className="font-bold"> "Hoje tem Festinha"</span>, <span className="font-bold">"Os Melhores de Gyn"</span> e 
                        <span className="font-bold"> "Cola no Automotivo"</span>, já colaborei com grandes nomes do cenário. Meu som é a vibe da noite, 
                        feito pra quem vive a energia das ruas e das festas.
                    </p>
                </section>
            );
        }

        function GallerySection() {
            return (
                <section className="max-w-4xl mx-auto p-6">
                    <h2 className="text-3xl font-bold mb-6 text-center glow-text">Galeria CADU NK</h2>
                    <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
                        <div className="overflow-hidden rounded-lg neon-border">
                            <img
                                src="https://drive.google.com/uc?export=download&id=1-PpTuJOJvu_yRXN2Knu-o9X6e0wb91dI"
                                alt="CADU NK em camiseta amarela"
                                className="w-full h-64 object-cover gallery-img"
                            />
                        </div>
                        <div className="overflow-hidden rounded-lg neon-border">
                            <img
                                src="https://drive.google.com/uc?export=download&id=1-VmnSI5yglxm0-tVgwPRxODVNRmvKuC3"
                                alt="CADU NK em camiseta preta"
                                className="w-full h-64 object-cover gallery-img"
                            />
                        </div>
                        <div className="overflow-hidden rounded-lg neon-border">
                            <img
                                src="https://drive.google.com/uc?export=download&id=1KQYBGrk6AhsHrnasagBilbU1VdnOBTv5"
                                alt="CADU NK em camisa do Brasil"
                                className="w-full h-64 object-cover gallery-img"
                            />
                        </div>
                    </div>
                </section>
            );
        }

        function MusicSection() {
            return (
                <section className="max-w-4xl mx-auto p-6">
                    <h2 className="text-3xl font-bold mb-6 text-center glow-text">Músicas em Destaque</h2>
                    <div className="grid grid-cols-1 md:grid-cols-3 gap-6">
                        <div className="p-4 bg-gray-900 rounded-lg neon-border">
                            <h3 className="text-xl font-bold">Hoje tem Festinha</h3>
                            <p className="mt-2">Um hino das noites de Goiânia, trazendo a energia do eletro funk.</p>
                            <a
                                href="https://open.spotify.com/track/1aQUURS7n8JvPxZUB0gRCE?si=IKK-UBqlQn6rQBOqG_iD_g"
                                target="_blank"
                                className="inline-block mt-4 px-6 py-3 bg-green-600 rounded-lg hover:bg-green-700 neon-border"
                            >
                                Ouvir no Spotify
                            </a>
                        </div>
                        <div className="p-4 bg-gray-900 rounded-lg neon-border">
                            <h3 className="text-xl font-bold">Os Melhores de Gyn</h3>
                            <p className="mt-2">O som que representa a cena de Goiânia com grave pesado.</p>
                            <a
                                href="https://open.spotify.com/track/64vRAqn78BbwdeU6eN18GF?si=XShemybCS1SCkM1qTNxzoQ"
                                target="_blank"
                                className="inline-block mt-4 px-6 py-3 bg-green-600 rounded-lg hover:bg-green-700 neon-border"
                            >
                                Ouvir no Spotify
                            </a>
                        </div>
                        <div className="p-4 bg-gray-900 rounded-lg neon-border">
                            <h3 className="text-xl font-bold">Cola no Automotivo</h3>
                            <p className="mt-2">Collab com grandes artistas, perfeito pra curtir no rolê.</p>
                            <a
                                href="https://open.spotify.com/album/5jtH14dJwHdMPqjefZvUyS?si=QJ0mt20SQKuQZaSFrJD7KQ"
                                target="_blank"
                                className="inline-block mt-4 px-6 py-3 bg-green-600 rounded-lg hover:bg-green-700 neon-border"
                            >
                                Ouvir no Spotify
                            </a>
                        </div>
                    </div>
                </section>
            );
        }

        function VideoSection() {
            return (
                <section className="max-w-4xl mx-auto p-6">
                    <h2 className="text-3xl font-bold mb-6 text-center glow-text">Videoclipe em Destaque</h2>
                    <div className="relative pb-9/16">
                        <iframe
                            className="w-full h-96 rounded-lg neon-border"
                            src="https://www.youtube.com/embed/B5pTtJDOfTQ"
                            title="CADU NK - Videoclipe"
                            frameBorder="0"
                            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                            allowFullScreen
                        ></iframe>
                    </div>
                </section>
            );
        }

        function Contact() {
            return (
                <section className="max-w-4xl mx-auto p-6 text-center">
                    <h2 className="text-3xl font-bold mb-6 glow-text">Contato</h2>
                    <p className="text-lg mb-4">Quer me contratar ou colaborar? Fala comigo!</p>
                    <div className="flex justify-center gap-6">
                        <a href="mailto:cadunk04@gmail.com" className="text-lg hover:text-pink-500">cadunk04@gmail.com</a>
                        <a href="tel:+5562993571882" className="text-lg hover:text-pink-500">(62) 99357-1882</a>
                    </div>
                    <div className="mt-6">
                        <a
                            href="https://www.instagram.com/ocadu.nk"
                            target="_blank"
                            className="inline-block px-6 py-3 bg-pink-600 rounded-lg hover:bg-pink-700 neon-border"
                        >
                            Instagram
                        </a>
                        <a
                            href="https://open.spotify.com/artist/1v7EtuWXY99NL4WJZxsAjo?si=om5YbPraQ4elnLLHWizkjQ"
                            target="_blank"
                            className="inline-block px-6 py-3 bg-green-600 rounded-lg hover:bg-green-700 neon-border ml-4"
                        >
                            Spotify
                        </a>
                    </div>
                </section>
            );
        }

        function Footer() {
            return (
                <footer className="py-6 text-center">
                    <p>© 2025 CADU NK. Todos os direitos reservados.</p>
                </footer>
            );
        }

        function App() {
            return (
                <div>
                    <Header />
                    <Bio />
                    <GallerySection />
                    <MusicSection />
                    <VideoSection />
                    <Contact />
                    <Footer />
                </div>
            );
        }

        const root = ReactDOM.createRoot(document.getElementById('root'));
        root.render(<App />);
    </script>
</body>
</html>
