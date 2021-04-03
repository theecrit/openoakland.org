---
title: Our Projects
date:  2020-11-19T07:50:52+00:00
author: Jess Sand
layout: page
scripts: ["/assets/js/project_filter.js"]
badges:
  brigade ops: 'success'
  incubating: 'info'
  active: 'success'
  dormant: 'primary'
  delivered: 'secondary'
  decommissioned: 'dark'
---

[Projects](#projects)  
[Becoming an OpenOakland project](#becoming-an-openoakland-project)  
[Providing feedback](#providing-feedback)  

---

## Projects

The following are official OpenOakland projects that are being actively supported by an existing team. If you see something that interests you, there are a couple of ways you can get involved:

- Join us for our Tuesday [Hack Nights](https://www.meetup.com/OpenOakland/events/) to connect with the project team.
- Join our [Slack workspace](https://join.slack.com/t/openoakland/shared_invite/zt-n4d7tx2t-UVIN7a769e4oc9j7PgM3HA) and introduce yourself in the project's channel listed in the description (see our [OpenOakland Slack Guide](https://docs.google.com/document/d/1VWZQ_3ehP5j0IOTY0nJClvQPll3ivSkuAdh5YsOhO_U/edit?usp=sharing) for help).

<project-filter>
  <div class="project-filter__toolbar"></div>

  <!-- Brigade ops -->
  {% for project in site.data.ops_projects %}
  {% assign status = 'brigade ops' %}
  {% include project.html %}
  {% endfor %}

  <!-- Active -->
  {% for project in site.data.active_projects %}
  {% assign status = 'active' %}
  {% include project.html %}
  {% endfor %}

  <!-- Incubating -->
  {% for project in site.data.incubating_projects %}
  {% assign status = 'incubating' %}
  {% include project.html %}
  {% endfor %}

  <!-- Idle -->
  {% for project in site.data.dormant_projects %}
  {% assign status = 'dormant' %}
  {% include project.html %}
  {% endfor %}

  <!-- Delivered -->
  {% for project in site.data.delivered_projects %}
  {% assign status = 'delivered' %}
  {% include project.html %}
  {% endfor %}

  <!-- Decommissioned -->
  {% for project in site.data.decommissioned_projects %}
  {% assign status = 'decommissioned' %}
  {% include project.html %}
  {% endfor %}
</project-filter>

---

## Becoming an OpenOakland project

OpenOakland is reevaluating how our projects are vetted, adopted, and developed. This is an ongoing pilot that we continue to iterate on in an effort to ensure that projects serve their intended communities, consider potential unintended consequences, and foster greater inclusion of community voices—particularly those from underrepresented and underserved Oakland communities.

If you have a new idea for an OpenOakland project:

1. **Fill out the [project exploration worksheet](https://docs.google.com/document/d/1k24P9JiAUEzJLPFRDjVh7aRZexax6NUhfPFLSI3R80M/edit?usp=sharing)**. We encourage you to join our [Slack workspace](https://join.slack.com/t/openoakland/shared_invite/zt-n4d7tx2t-UVIN7a769e4oc9j7PgM3HA) and share your draft with our membership, so we can collaborate together as you develop your idea.

2. **Submit your draft brief to the #oo-steering-committee channel** on Slack for formal consideration. Provided your brief is submitted at least two weeks in advance, it will be reviewed at the next Steering Committee meeting (a group of elected leadership and existing project reps), and you'll get some initial feedback and be asked to make adjustments accordingly.

3. **Make any requested adjustments** based on the Steering Committee's feedback and resubmit the final brief.

Once your final brief is submitted, the Steering Committee will hold a formal vote to approve or decline the project.

### What makes a good project?

We generally consider the following types of projects:

- **Civic tech projects:** providing tools or services to Oaklanders or public agencies to increase access to and understanding of government.
- **Events:** major events that require a team to execute.
- **OpenOakland sustainability projects:** efforts to improve and sustain OpenOakland as an organization.

Projects must demonstrate alignment to OpenOakland’s mission and values. Some ways a project might do so include:

- Partnering with organizations to serve as domain experts in the needs of the community it serves
- Forming a project team which has lived experience with the issue the project is focused on
- Conducting user research to understand the needs of the community the project serves

### Idle projects

Projects with the <span class="badge badge-{{ page.badges['inactive'] }}">Inactive</span> label have either served their purpose or are otherwise no longer actively supported. If you'd like to resume or adapt one of these, submit a [project exploration worksheet](https://docs.google.com/document/d/1k24P9JiAUEzJLPFRDjVh7aRZexax6NUhfPFLSI3R80M/edit?usp=sharing) at an upcoming Hack Night or in Slack's #leadership channel.

### Decommissioned projects

Projoects with the <span class="badge badge-{{ page.badges['decommissioned'] }}">Decommissioned</span> label are projects that the Steering Committee has formally reviewed and deemed no longer a good fit for OpenOakland based on our 2020 project evaluation pilot. These projects may not be reinstated without submitting a new [project exploration worksheet](https://docs.google.com/document/d/1k24P9JiAUEzJLPFRDjVh7aRZexax6NUhfPFLSI3R80M/edit?usp=sharing) that substantively addresses the original reasons for discontinuation. Project briefs that are declined by the Steering Committee twice may not be resubmitted without substantive changes.

---

## Providing feedback

In the spirit of continuous improvement and self-reflection, we welcome any and all feedback on OpenOakland projects past and present, as well as the overall project management process. Ways you can share your input include:

- Open an issue in the project's GitHub repository (listed in the project description).
- Join the project's channel in our [Slack workspace](https://join.slack.com/t/openoakland/shared_invite/zt-n4d7tx2t-UVIN7a769e4oc9j7PgM3HA) and introduce yourself (see our [OpenOakland Slack Guide](https://docs.google.com/document/d/1VWZQ_3ehP5j0IOTY0nJClvQPll3ivSkuAdh5YsOhO_U/edit?usp=sharing) for help).
- Join our next [Hack Night](https://www.meetup.com/OpenOakland/events/) and meet the team.
- Email our [Steering Committee](mailto:steering@openoakland.org) with your input.

You may also email concerns or comments to <safespace@openoakland.org>, which is staffed by two OpenOakland [ombudspeople](https://docs.google.com/document/d/1QR-fr1WnmXkZoVNmWnZ9drzfmaZoPkodEOx-PkExt94/edit#heading=h.3t0te9n2wr7m).
