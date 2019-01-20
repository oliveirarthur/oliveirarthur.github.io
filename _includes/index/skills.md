<div class="row align-items-center" id="skills">

  <div class="col py-3 text-center">
    <h2 class="py-2">Ferramentas e tecnologias</h2>

    <div class="row">
      {% for skill in site.data.skills %}
        <div class="col-sm-6 col-md-3 pb-3">
          <div class="card">
            <div class="card-header">{{ skill.title }}</div>
            <div class="card-body">
              {% for item in skill.items %}
                <div class="row align-items-center py-2">
                  <div class="col-3 col-md-4 col-lg-4 col-xl-3">
                    <img src="assets/img/skills/{{ skill.id }}/{{ item.icon }}"
                      class="img-fluid"
                      alt="{{ item.title }} logo">
                  </div>
                  <div class="col text-truncate">
                    {{ item.title }}
                  </div>
                </div>
              {% endfor %}
            </div>
          </div>
        </div>
      {% endfor %}
    </div>

  </div>
</div>
