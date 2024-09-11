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
                    Join us for the Camera Traps, AI, and Ecology workshop, part of an international series focusing on wildlife monitoring using AI and camera traps. This workshop, held both live and online, unites camera trap data producers, scientific practitioners, and AI providers to foster collaboration, bridge wildlife data with AI, and initiate interdisciplinary projects. 
                </p>
                <p class="bold">
                    We are excited to announce that the workshop schedule has been finalized! We invite you to take a look and plan your participation accordingly. <br/>
                    <a href="{{ site.baseurl }}/program" class="btn btn-primary">See the program!</a>
                </p>
                <p>
                Previous workshops were conducted in 2022 and 2023. Past content can be found at:
                <ul>
                    <li><a href="https://inf-cv.uni-jena.de/camtrap-ws/">2023 Workshop at the University Jena</a> </li>
                    <li>the <a href="https://camtrapai.github.io/indexold.html">Archive of the 1st and 2nd workshops</a></li>
                </ul>
                </p>
                <!--<p>
                    Stay updated on the 2024 workshop details on this site. For inquiries, feel free to <a href="#contact">contact us</a>.
                </p>
                <p>To join us online or in Hagenberg <br/>
                    <a href="https://events.teams.microsoft.com/event/1736783a-9476-4f7d-a3f4-927637d3f714@f88d4b73-6bb2-4b9a-abc7-eb96e5a6407c" class="btn btn-primary">Register (for free) now! <i class="fa fa-external-link" aria-hidden="true"></i></a>
                </p>-->
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
                    <li>Paper submission due:           <span><s>June 28, 2024</s> <!--<s>Extension: July 19, 2024</s> -->2ⁿᵈ Extension: July 31, 2024</span></li>
                    <li>Paper acceptance notification:  <span><s>August 10, 2024</s> August 18, 2024</span></li>
                    <li>Camera-ready version due:         <span><s>August 21, 2024</s> September 1, 2024</span></li>
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
                    <b>Online access</b> is available as Microsoft Teams Event (you need to accept the event)!
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
