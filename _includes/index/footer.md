<div class="card my-5">
  <div class="card-header text-center">
    <h5>Encontre-me nas redes sociais!</h5>
  </div>
  <div class="card-body text-center">
    {% for socialNetwork in .site.data.social-networks %}
      <a
        href="{{ socialNetwork.url }}"
        target="_blank"
        class="btn btn-default p-1 col-3 col-sm-2 col-lg-1"
        title="{{ socialNetwork.title }}"><i class="fa-3x {{ socialNetwork.icon }} p-2"></i><br>
        <p class="card-text text-truncate">{{ socialNetwork.title }}</p></a>
    {% endfor %}
  </div>
</div>
