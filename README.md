# aula-5-alura
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Tropicália - Acessível</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bootstrap-icons/1.11.3/font/bootstrap-icons.min.css">
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="bg-light border-bottom py-4">
        <nav class="container d-flex justify-content-between align-items-center">
            <img src=img/4965007.jpg"i" class="nav-img" alt="" loading="lazy">
            <ul class="nav mt-4">
                <li class="nav-item"><a class="nav-link link-dark fw-bold fs-5" href="#inicio">Início</a></li>
                <li class="nav-item"><a class="nav-link link-dark fw-bold fs-5" href="#galeria">Galeria</a></li>
                <li class="nav-item"><a class="nav-link link-dark fw-bold fs-5" href="#contato">Contato</a></li>
            </ul>
            <div id="acessibilidade" class="menu-acessibilidade">
                <button id="botao-acessibilidade" class="btn btn-outline-dark fw-bold" aria-expanded="false">Acessibilidade</button>
                <div id="opcoes-acessibilidade" class="opcoes-acessibilidade apresenta-lista">
                    <button id="aumentar-fonte" class="btn btn-dark fw-bold" aria-label="Aumentar o tamanho da fonte">A+</button>
                    <button id="diminuir-fonte" class="btn btn-dark fw-bold" aria-label="Diminuir o tamanho da fonte">A-</button>
                    <button id="alterna-contraste" class="btn btn-dark fw-bold" aria-label="Alternar o contraste de cores"><i class="bi bi-shadows"></i></button>
                </div>
            </div>
        </nav>
    </header>
    <main class="container my-5">
        <section id="inicio" class="my-5">
            <div class="inicio-fundo d-flex justify-content-between align-items-center bg-white p-4 rounded-4 shadow-sm">
                <div class="esquerda-conteudo">
                    <h1 class="display-4 text-dark fw-bold" style="font-family: 'Arial', sans-serif;">Boas-vindas a</h1>
                    <img src="img/logo-2.png" class="mb-3" width="400" height="180" loading="lazy" alt="Logo Tropicália Alternativa">
                    <a href="#tropicalia" class="btn btn-dark btn-lg botao-inicio fw-semibold">Quero conhecer!</a>
                </div>
                <img src="img/lossy-page1-640px-Os_Mutantes.tif (1).png" alt="O grupo musical Os Mutantes, três pessoas cantando em um microfone" class="img-fluid img-inicio rounded-4 shadow-sm">
            </div>
        </section>
        <section id="tropicalia" class="my-5 pt-6 secao-tropicalia" tabindex="0" aria-label="Seção explicativa sobre a tropicália">
            <div class="container d-flex align-items-center">
                <div class="col-4 d-flex justify-content-center">
                    <img src="img/image (1).png" class="rounded-pill shadow-sm" width="220" height="260" loading="lazy" alt="Imagem ilustrativa Tropicália">
                </div>
                <div class="col-7">
                    <h2 class="fw-bold text-dark">O que foi a Tropicália?</h2>
                    <p class="p-2 fs-5 text-dark" style="font-family: 'Arial', sans-serif;">
                        A Tropicália, também conhecida como Tropicalismo, foi um movimento cultural brasileiro que surgiu na década de 1960, tendo seu auge entre 1967 e 1968. Esse movimento abrangeu várias expressões artísticas, como a música, o cinema, o teatro e as artes plásticas, e teve como principal característica a mistura de elementos da cultura brasileira tradicional com influências estrangeiras, especialmente do rock e da música pop.
                        <br><small class="text-secondary">Fonte: Site Toda a matéria</small>
                    </p>
                </div>
            </div>
        </section>
        <section id="galeria" tabindex="0" aria-label="Seção de galeria de imagens">
            <h2 class="text-center pt-5 fw-bold text-dark">Galeria</h2>
            <div class="container p-3 mt-3 fundo-galeria bg-white rounded-4 shadow-sm">
                <div class="row justify-content-md-center">
                    <div class="col-md-4 mb-3">
                        <img src="img/lossy-page1-640px-Jorge_Ben_e_o_Trio_Mocotó_no_Teatro_da_Lagoa,_1971.tif.jpg"
                            class="img-fluid rounded-4 shadow-sm" loading="lazy" alt="Jorge Ben e Trio Mocotó">
                    </div>
                    <div class="col-md-4 mb-3">
                        <img src="img/lossy-page1-640px-Os_Mutantes_2.tif.jpg" class="img-fluid rounded-4 shadow-sm"
                            loading="lazy" alt="Os Mutantes">
                    </div>
                </div>
                <div class="row mt-4 justify-content-md-center">
                    <div class="col-md-4 mb-3">
                        <img src="img/lossy-page1-640px-Gilberto_Gil_nos_anos_1960.tif.jpg" class="img-fluid rounded-4 shadow-sm" loading="lazy" alt="Gilberto Gil">
                    </div>
                    <div class="col-md-4 mb-3">
                        <img src="img/lossy-page1-640px-Caetano_Veloso_no_III_Festival_da_Música_Popular.tif.jpg"
                            class="img-fluid rounded-4 shadow-sm" loading="lazy" alt="Caetano Veloso">
                    </div>
                </div>
            </div>
        </section>
        <section id="contato" class="my-5">
            <div class="container p-5 d-flex justify-content-center">
                <div class="col-md-8 col-lg-10 rounded-4 formulario bg-white shadow-sm">
                    <h2 class="mb-3 fw-bold text-dark">Entre em contato</h2>
                    <form>
                        <div class="form-group mb-3">
                            <label for="nome" class="fw-bold text-dark">Nome</label>
                            <input type="text" id="nome" name="nome" class="form-control rounded-3 mt-1"
                                placeholder="Digite seu nome completo" required style="font-size:18px;">
                        </div>
                        <div class="form-group mb-3">
                            <label for="email" class="fw-bold text-dark">Email</label>
                            <input type="email" id="email" name="email" class="form-control rounded-3 mt-1"
                                placeholder="Digite seu email" required style="font-size:18px;">
                        </div>
                        <div class="form-group mb-3">
                            <label for="mensagem" class="fw-bold text-dark">Mensagem</label>
                            <textarea id="mensagem" name="mensagem" class="form-control rounded-3 mt-2" rows="4"
                                placeholder="Escreva sua mensagem" required style="font-size:18px;"></textarea>
                        </div>
                        <div class="d-grid gap-2">
                            <button type="submit" class="btn btn-dark btn-lg rounded-pill">Enviar mensagem</button>
                        </div>
                    </form>
                </div>
            </div>
        </section>
    </main>
    <footer class="text-center p-3 bg-light border-top fst-italic">
        <p class="fw-bold text-dark">Acesse nossas redes:</p>
        <i class="bi bi-whatsapp fs-3 mx-2 text-dark"></i>
        <i class="bi bi-instagram fs-3 mx-2 text-dark"></i>
        <i class="bi bi-tiktok fs-3 mx-2 text-dark"></i>
        <p class="mt-3 text-secondary">Desenvolvido por Thayla Bomfim. Projeto fictício sem fins comerciais.</p>
    </footer>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/scrollReveal.js/4.0.9/scrollreveal.js"></script>
    <script src="script.js"></script>
</body>
</html>