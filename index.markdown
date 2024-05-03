---
layout: home
lang: en
permalink: /
description: Homepage of the Camera Traps, AI, and Ecology Workshop 2024
---

<section class="background-light pad" id="welcome">
    <div class="container text-justify"> 
        <div class="row">
            <div class="col-lg-12 col-md-12">
                <h1>Information</h1>
                <p class="text-justify">
                    The workshop on Camera traps, AI, and Ecology is held as a part of the international workshop series on camera traps and AI analysis for wildlife monitoring, including associated ecological and data collection methods. It runs as live and online sessions of expert talks, tutorials, discussions, and follow-up sessions. The workshop brings together three communities: camera trap data producers (e.g., nature parks and reserves), scientific practitioners (e.g., ecologists and conservationists), and AI analysis providers (e.g., computer scientists and engineers). The aim of the workshop is to promote exchange between these different communities, link wildlife data and AI methods, and initiate new interdisciplinary projects amongst attendees.
                </p>
                <p>
                The previous three workshops were held in 2022 and 2023. Content of previous workshops is available at
                <ul>
                    <li>the <a href="https://inf-cv.uni-jena.de/camtrap-ws/">2023 Workshop at the University Jena</a>, and </li>
                    <li>the <a href="https://camtrapai.github.io/indexold.html">Archive of the 1st and 2nd workshops</a>.</li>
                </ul>
                </p>
                <p>
                    All information regarding the organization of the 2024 workshop is provided and will be constantly updated on this website. In case of any additional inquiries, please do not hesitate to <a href="#contact">contact us</a>.
                </p>
                <br/>
                <p>See you soon at our workshop &ndash; online or in Hagenberg, Austria!</p>
            </div>
        </div>
    </div>
</section>

<section class="background-primary pad" id="calls">
    <div class="container text-justify">
        <div class="row">
            <div class="col-lg-6 col-md-12">
                <h2>Dates and Deadlines</h2>
                <p class="text-justify">
                    The workshop will take place from <b>September 5-6, 2024</b>. Other important dates are:<br/>
                </p>
                <ul class="date-list">
                    <li>Paper submission due:           <span>June 28, 2024</span></li>
                    <li>Paper acceptance notification:  <span>August 10, 2024</span></li>
                    <li>Camera-ready version due:         <span>August 21, 2024</span></li>
                </ul>
                <p>
                    <em>(deadline interpretation = end of the day, anywhere on earth)</em> <br/>
                    For further details look at <a href="{{ site.baseurl }}/calls">Calls</a> and <a href="{{ site.baseurl }}/program">Program</a>.
                </p>
            </div>
            <div class="col-lg-6 col-md-12">
                <h2>Online and On-site</h2>
                <p class="text-justify">
                    The on-site venue is the Campus of the <b>University of Applied Sciences Upper Austria</b>, located in <a href="{{ site.baseurl }}/venue"><b>Hagenberg, Austria</b></a>.
                </p>
                <p>
                    <address>
                    University of Applied Sciences Upper Austria<br/>
                    Softwarepark 11<br/>
                    4232 Hagenberg im Mühlkreis<br/>
                    Austria
                    </address>
                </p>
                <p>
                    Further details about the <b>online access</b> will be announced shortly before the workshop!
                </p>
            </div>
        </div>
    </div>
</section>

<section class="background-light pad" id="contact">
   <div class="container text-justify">
      <div class="row"><div class="col-sm-12">Write us at <a style="text-decoration:underline" href="mailto:camtraps2024@fh-hagenberg.at">camtraps2024@fh-hagenberg.at</a>.<br/><br/></div></div>
      <h2>Local Organization Team</h2>
      <div class="row contact-info">
         {% for group in site.data.people.groups %}
         {% if group.short == "fhooe" %}
         {% for member in group.members %}
         {% if member.contact %}
         <div class="col-lg-4 col-md-12">
            <h4>{{member.prefix}} {{member.firstname}} {{member.lastname}} {{member.postfix}}</h4>
            <p>{{member.organization}}<br>{{member.phone}}</p>
            <!--<table class="contact-table">
               <body>
                  <tr>
                     <td>Phone:</td>
                     <td>{{member.phone}}</td>
                  </tr>
                  <tr>
                     <td>Mail:</td>
                     <td>
                        <a href="mailto:{{member.mail}}">{{member.mail}}</a>
                     </td>
                  </tr>
               </body>
            </table> -->
         </div>
         {% endif %}
         {% endfor%}
         {% endif %}
         {% endfor %}
      </div>
      <h2>Workshop Series Organizers</h2>
      <div class="row contact-info">
         {% for group in site.data.people.groups %}
         {% if group.short == "camtrap" %}
         {% for member in group.members %}
         {% if member.contact %}
         <div class="col-lg-4 col-md-12">
            <h4>{{member.prefix}} {{member.firstname}} {{member.lastname}} {{member.postfix}}</h4>
            <p>{{member.organization}}<br>{{member.phone}}</p>
            <!--<table class="contact-table">
               <body>
                  <tr>
                     <td>Phone:</td>
                     <td>{{member.phone}}</td>
                  </tr>
                  <tr>
                     <td>Mail:</td>
                     <td>
                        <a href="mailto:{{member.mail}}">{{member.mail}}</a>
                     </td>
                  </tr>
               </body>
            </table> -->
         </div>
         {% endif %}
         {% endfor%}
         {% endif %}
         {% endfor %}
      </div>
      <!-- link to the team subpage -->
      <div class="row">
            <div class="col-sm-12">
            For more information about the team and organizers, please visit the <a href="{{ site.baseurl }}/team">Team</a> page.
            </div>
      </div>
   </div>
</section>

{% include map.html %}
