<template>
  <main class="resume">
    <div class="resume__main">
      <header class="resume__header">
        <div class="resume__monogram" aria-label="Iniciais MM">MM</div>
        <div class="resume__identity">
          <h1>Marty McFly</h1>
          <p>Consultor de Cronologia e Especialista em Performance Musical</p>
        </div>
      </header>

      <section class="resume__intro" aria-label="Resumo profissional">
        <p>
          Jovem dinâmico, pontual (quando o capacitor de fluxo permite) e com vasta experiência em
          resolução de paradoxos temporais. Guitarrista talentoso com domínio de técnicas avançadas
          de shredding antes mesmo de serem inventadas. Experiente em lidar com figuras históricas,
          direção defensiva de veículos modificados e skate urbano. Nota: Não me chame de frangote.
        </p>
      </section>

      <section class="resume__experience">
        <h2 class="section-label">Experiências profissionais</h2>

        <article class="resume__item">
          <h3>1985 – Presente | The Pinheads</h3>
          <p class="resume__role">Guitarrista Principal</p>
          <p>
            Composição e performance de Rock 'n' Roll. Responsável pela audição da "Batalha das
            Bandas" (mesmo sendo considerado "barulhento demais" por alguns juízes).
          </p>
        </article>

        <article class="resume__item">
          <h3>1955 – Baile Encanto sob o Mar</h3>
          <p class="resume__role">Músico Substituto (Guitarra)</p>
          <p>
            Substituição emergencial do guitarrista Marvin Berry. Responsável pela introdução
            cultural do gênero Heavy Metal trinta anos antes do previsto.
          </p>
        </article>

        <article class="resume__item">
          <h3>1885 – Consultoria de Segurança Hill Valley (Velho Oeste)</h3>
          <p class="resume__role">Assistente de Ferreiro</p>
          <p>
            Auxílio técnico em engenharia ferroviária improvisada e mediação de conflitos com a
            gangue de Buford "Cachorro Louco" Tannen.
          </p>
        </article>

        <article class="resume__item">
          <h3>1985 – Indústrias Biffco</h3>
          <p class="resume__role">Sobrevivente Urbano</p>
          <p>
            Gestão de crises em ambientes distópicos e recuperação de artefatos esportivos
            (almanaques) para restauração da ordem cronológica.
          </p>
        </article>
      </section>

      <footer class="resume__footer">
        <p>Copyright 2026 - todos os direitos reservados</p>
      </footer>
    </div>

    <aside class="resume__sidebar">
      <section class="resume__education">
        <h2 class="section-label">Educação</h2>

        <article class="resume__item">
          <h3>1986 | Hill Valley High School</h3>
          <p class="resume__role">Ensino Médio Completo</p>
          <p>Foco em Artes e Música</p>
        </article>

        <article class="resume__item">
          <h3>1955 | Cultural Hill Valley</h3>
          <p class="resume__role">Intercâmbio</p>
          <p>Estudos intensivos sobre dinâmicas sociais da década de 50 e etiqueta de lanchonetes.</p>
        </article>

        <article class="resume__item">
          <h3>1985 | Engenharia Aplicada</h3>
          <p class="resume__role">Workshop</p>
          <p>
            Treinamento prático em sistemas de 1.21 Gigawatts e mecânica de DeLorean (sob mentoria
            do Dr. Emmett Brown).
          </p>
        </article>

        <article class="resume__item">
          <h3>2015 | Mobilidade Urbana Futurista</h3>
          <p class="resume__role">Treinamento</p>
          <p>
            Curso intensivo de pilotagem de Hoverboard em superfícies sólidas (atenção: pranchas não
            funcionam na água sem potência extra).
          </p>
        </article>
      </section>

      <section class="resume__contact">
        <h2 class="section-label">Contato</h2>
        <p><strong>Endereço:</strong> Lyon Estates, Hill Valley, CA.</p>
        <p><strong>E-mail:</strong> contato@delorean.com</p>
        <p><strong>Telefone:</strong> +55 (88) 9999 0000</p>
      </section>
    </aside>
  </main>
</template>

<style scoped>
:global(*) {
  box-sizing: border-box;
}

:global(body) {
  margin: 0;
  background: #f3f3f3;
  color: #171717;
  font-family: Arial, Helvetica, sans-serif;
}

.resume {
  display: grid;
  grid-template-columns: minmax(0, 2fr) minmax(0, 1fr);
  width: min(100%, 960px);
  min-height: 100vh;
  margin: 0 auto;
  padding: 46px 25px 32px;
  border: 1px solid #222;
  background: #fff;
}

.resume__main {
  display: flex;
  min-width: 0;
  flex-direction: column;
  padding-right: 25px;
}

.resume__header {
  display: flex;
  align-items: center;
  gap: 17px;
}

.resume__monogram {
  display: grid;
  width: 64px;
  height: 64px;
  flex: 0 0 64px;
  place-items: center;
  background: #f0d62e;
  font-size: 30px;
  font-weight: 700;
}

.resume__identity h1 {
  margin: 0 0 7px;
  font-family: "Courier New", monospace;
  font-size: 13px;
  font-weight: 700;
}

.resume__identity p {
  font-family: "Courier New", monospace;
  font-size: 9px;
}

.resume__intro {
  margin-top: 21px;
}

.resume__intro p,
.resume__item > p:not(.resume__role) {
  font-size: 10px;
  line-height: 1.9;
}

.resume__experience {
  margin-top: 24px;
}

.section-label {
  margin: 0 0 22px;
  color: #c3c3c3;
  font-size: 8px;
  font-weight: 700;
  letter-spacing: 1.5px;
  line-height: 1.5;
  text-transform: uppercase;
}

.resume__item {
  margin-bottom: 27px;
}

.resume__item h3 {
  margin: 0 0 9px;
  font-size: 10px;
  font-weight: 700;
  line-height: 1.5;
}

.resume__role {
  margin: 0 0 7px;
  color: #858585;
  font-family: "Courier New", monospace;
  font-size: 10px;
  font-weight: 700;
  line-height: 1.5;
}

.resume__sidebar {
  min-width: 0;
  padding: 20px 0 0 22px;
  border-left: 1px solid #ededed;
}

.resume__sidebar .section-label {
  margin-bottom: 22px;
}

.resume__sidebar .resume__item {
  margin-bottom: 25px;
}

.resume__contact {
  margin-top: 2px;
  padding-top: 20px;
  border-top: 1px solid #ededed;
}

.resume__contact .section-label {
  margin-bottom: 17px;
}

.resume__contact p {
  margin-bottom: 8px;
  font-size: 8px;
  line-height: 1.5;
}

.resume__contact strong {
  font-weight: 700;
  text-transform: uppercase;
}

.resume__footer {
  margin-top: auto;
  padding-top: 38px;
  border-top: 1px solid #f1f1f1;
}

.resume__footer p {
  color: #c3c3c3;
  font-size: 8px;
  font-weight: 700;
  letter-spacing: 1px;
  text-transform: uppercase;
}

@media (max-width: 640px) {
  .resume {
    grid-template-columns: 1fr;
    padding: 28px 20px;
  }

  .resume__main {
    padding-right: 0;
  }

  .resume__sidebar {
    margin-top: 8px;
    padding: 25px 0 0;
    border-top: 1px solid #ededed;
    border-left: 0;
  }

  .resume__footer {
    margin-top: 16px;
  }
}

@media (max-width: 400px) {
  .resume {
    padding-right: 16px;
    padding-left: 16px;
  }

  .resume__header {
    align-items: flex-start;
    gap: 12px;
  }

  .resume__monogram {
    width: 56px;
    height: 56px;
    flex-basis: 56px;
    font-size: 26px;
  }

  .resume__identity p {
    line-height: 1.5;
  }
}
</style>
