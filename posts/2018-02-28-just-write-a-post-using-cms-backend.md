---
title: just write a post using cms backend
layout: post
date: 2018-02-28T15:05:36.727Z
---
Git Gateway is a Netlify open source project that allows you to add editors to your site CMS without giving them direct push access to your GitHub repository. Netlify Identity service handles the authentication and provides a simple interface for user management. The Netlify CMS featured templates are working examples of this backend.



To use it in your own project, follow these steps:



Head over to the Netlify Identity docs and follow the steps to get started.

Add the following lines to your config.yml file:



backend:

  name: git-gateway

  accept_roles: #optional - accepts all users if left out

\- admin

\- editor

\    

Optionally, you can assign roles to users in your Netlify dashboard, and then limit which roles can access the CMS by defining the accept_roles field in the config.yml example above. Otherwise accept_roles can be left out, and all Netlify Identity users on your site will have access.
