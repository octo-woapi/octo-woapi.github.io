---
layout: default
---
<div id="grid" class="row flex-grid">
    {% for post in site.posts %}
        <article class="box-item post-{{post.main-class}}">
            <span class="ribbon"><span>{{post.main-class}}</span>
            </span>
            <div class="box-body">
                <h2 class="post-title" itemprop="name">
                    {{ post.title }}
                </h2>
                    <p class="description">{{ post.description }}</p>
            </div>
            <div class="box-image">
              <img src="/images/GitHub-Mark.png" class="project-github-image">
            </div>
        </article>
    {% endfor %}
</div>
