---
layout: default
style: cv
container: default
---

{% assign age = 'now' | date: "%Y" | minus: 1995 %}

<h1>
  <center>Arthur Mendes de Oliveira</center>
</h1>

<div class="overview mt-3">
  <div class="row">
    <div class="col">{{ age }} anos, solteiro</div>
    <div class="col">
      <a href="tel:(15) 9 8176 1164">(15) 9 8176 1164</a>
    </div>
  </div>
  <div class="row">
    <div class="col">Sorocaba/SP</div>
    <div class="col">
      <a href="tel:(19) 9 9839 2636">(19) 9 9839 2636</a>
    </div>
  </div>
  <div class="row">
    <div class="col"></div>
    <div class="col">
      <a href="mailto:arthur.oliveira@hotmail.com.br">arthur.oliveira@hotmail.com.br</a>
    </div>
  </div>
</div>

---

## Formação acadêmica

- FATEC José Crespo Gonzales - Centro Paula Souza
  - Tecnólogo em análise e desenvolvimento de sistemas <small>(concluído)</small>  
      de 1º sem. 2014 ao 2º sem 2017
- ETEC Prefeito Alberto Feres - Centro Paula Souza
  - Técnico em informática para internet <small>(concluído)</small>  
      de 1º sem. 2012 ao 1º sem. 2013

## Experiência profissional
- Analista Desenvolvedor - FIT <small>(CLT)</small> (Março/2019 - Atualmente)
  - Desenvolvimento de aplicaçôes utilizando Angular e outras ferramentas.
- Analista Desenvolvedor <small>(PJ)</small> (Maio/2017 - Março/2019)
  - Desenvolvimento de projetos web envolvendo diversas tecnologias.
- Estágio - GFT Tecnologies (Maio/2016 - Maio/2017)
  - Desenvolvimento de aplicações utilizando metodologia Scrum e as tecnologias Java, Hibernate, Spring MVC, Oracle DB, HTML5, CSS3, AngularJS, Angular 2 e Bootstrap.
- Freelancer
  - Desenvolvimento de aplicações web utilizando APIs RESTful, Angular 2+, Foundation 6, Bootstrap, Ionic 2, Laravel, Lumen, PHP 7, gulp, Sass e MySQL.

## Outros conhecimentos
- Controle de versão de código com Git;
- Tecnologias como NodeJS, Typescript, ShellScript, Docker e Vagrant; além dos frameworks AdonisJS ExpressJS, CakePHP, Zend Framework 2 e CodeIgniter;
- Conhecimento em Linux;
- Experiência com infraestrutura utilizando Amazon Web Services e Firebase;
- Inglês nível intermediário para leitura e básico para conversação.

<footer class="text-right small">
  Arquivo atualizado em {{ 'now' | date: "%Y-%m-%d %H:%M" }}
</footer>
