### Hi there 👋

 {{ with $person.education }}
      <div class="col-md-7">
        <h3>{{ i18n "education" | markdownify }}</h3>
        <ul class="ul-edu fa-ul">
          {{ range .courses }}
          <li>
            <!--https://github.com/catrincm/personal-website/blob/e06b3525f51a3dd2653578a29c9b5b253596ab1a/layouts/partials/widgets/about.html-->
            {{ if .course }}
            <i class="fa-li fas fa-graduation-cap"></i>
            <div class="description">
              <p class="course">{{ .course }}{{ with .year }}, {{ . }}{{ end }}</p>
              <p class="institution">{{ .institution | markdownify }}</p>
              <!--https://github.com/gcushen/hugo-academic/issues/1094#issuecomment-622200594-->
            </div>
            {{ end }}
            {{ if .certificate }}
            <i class="fa-li fas fa-certificate"></i>
            <div class="description">
              <p class="course">{{ .certificate }}{{ with .year }}, {{ . }}{{ end }}</p>
              <p class="institution">{{ .institution | markdownify }}</p>
              <!--https://github.com/gcushen/hugo-academic/pull/951#issue-255104712-->
            </div>
            {{ end }}

          </li>
          {{ end }}
        </ul>
      </div>
      {{ end }}
<!--
**seyed-mohammadreza-mousavi/seyed-mohammadreza-mousavi** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
