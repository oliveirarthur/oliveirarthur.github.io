<div class="card my-5 text-center skills">
  <div class="card-header">
    <h5>Habilidades técnicas</h5>
    <ul class="nav nav-tabs nav-fill card-header-tabs">
      {% for skill in site.data.skills %}
        <li class="nav-item">
          <a
            class="nav-link {% if forloop.first %} active {% endif %}"
            id="{{ skill.id }}-tab"
            data-toggle="tab"
            href="#{{ skill.id }}"
            role="tab"
            aria-controls="{{ skill.id }}"
            aria-selected="false">{{ skill.title }}</a>
        </li>
      {% endfor %}
    </ul>
  </div>
  <div class="card-body">
    <div class="tab-content">
      {% for skill in site.data.skills %}
        <div
          class="tab-pane fade {% if forloop.first %} show active {% endif %}"
          id="{{ skill.id }}"
          role="tabpanel"
          aria-labelledby="{{ skill.id }}-tab">
          <div class="row justify-content-around">
            {% for item in skill.items %}
              <div class="col">
                <div class="card border-0">
                  <img class="card-img-top py-2" src="assets/img/skills/{{ skill.id }}/{{ item.icon }}" alt="Card image cap">
                  <div class="card-body p-0 text-center">
                    <h5 class="card-title text-truncate py-1">{{ item.title }}</h5>
                  </div>
                </div>
              </div>
            {% endfor %}
          </div>
        </div>
      {% endfor %}
    </div>
  </div>
</div>
