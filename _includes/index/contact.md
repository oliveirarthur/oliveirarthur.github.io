<div class="card contact my-5">
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
          class="form-text text-muted">Se preferir, insira seu WhatsApp. Ah, e não se esqueça de inserir o DDD!</small>
      </div>
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
<script defer>
  $('form.contact').on('submit', function() {
    var message = $('form.contact #message');
    setTimeout(function() {
      message.val('');
      message.focus();
    }, 1000);
  });
</script>
