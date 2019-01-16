<div class="row align-items-center" id="contact">

  <div class="col-xs-12 col-lg-6 py-3 text-center">
    <div class="card my-5">
      <div class="card-header text-center">
        <h5>Contato</h5>
      </div>
      <form class="contact mb-0" action="{{ site.contact-form.url }}/formResponse" method="post" target="_blank">
        <div class="card-body">
          <div class="form-group">
            <label for="name">Nome *</label>
            <input
            name="entry.1242810783"
            type="text"
            class="form-control"
            id="name"
            placeholder="Insira seu nome"
            required>
          </div>
          <div class="form-group">
            <label for="email">Email *</label>
            <input
            name="entry.2111747652"
            type="email"
            class="form-control"
            id="email"
            placeholder="Qual seu email?"
            required>
          </div>
          <div class="form-group">
            <label for="phone">Telefone</label>
            <input
            name="entry.562096638"
            type="text"
            class="form-control"
            id="phone"
            placeholder="Telefone para contato"
            aria-describedby="phone-help">
            <small
            id="phone-help"
            class="form-text text-muted">Opcional! E se preferir, insira seu WhatsApp. Ah, e não se esqueça de inserir o DDD!</small>
          </div>
          <hr>
          <div class="form-group">
            <label for="message">Mensagem *</label>
            <textarea
            name="entry.1349482598"
            class="form-control"
            id="message"
            rows="3"
            placeholder="Mensagem"></textarea>
          </div>
        </div>
        <div class="card-footer">
          <button type="submit" class="btn btn-primary btn-block">Enviar</button>
        </div>
      </form>
    </div>
  </div>

  <div class="col-xs-12 col-lg-6 py-3 text-center">
    <div class="card my-5">
      <div class="card-header text-center">
        <h5>Encontre-me nas redes sociais!</h5>
      </div>
      <div class="card-body text-center">
        {% for socialNetwork in .site.data.social-networks %}
          <a
            href="{{ socialNetwork.url }}"
            target="_blank"
            class="btn btn-default p-1 col-xs-3 col-sm-4 col-lg-2"
            title="{{ socialNetwork.title }}"><i class="fa-3x {{ socialNetwork.icon }} p-2"></i><br>
            <p class="card-text text-truncate">{{ socialNetwork.title }}</p></a>
        {% endfor %}
      </div>
    </div>
  </div>

</div>
<script defer>
  $('form.contact').on('submit', function() {
    var message = $('form.contact #message');
    setTimeout(function() {
      message.val('');
      message.focus();
    }, 1000);
  });
</script>
