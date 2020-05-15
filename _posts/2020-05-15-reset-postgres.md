---
title: 'How to reset the PostgreSQL database in Django?'
date: 2020-05-15
permalink: /posts/2020/05/blog-post-1/
tags:
  - Notes
  - Django
  - Stackoverflow
---

    sudo su postgres
    psql
    drop database database_test;
    create database database_test with owner suresh;
    \q
    exit

    python manage.py migrate
