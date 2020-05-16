---
title: 'How to delete a record in Django models'
date: 2020-05-16
permalink: /posts/2020/05/blog-post-2/
tags:
  - Notes
  - Django
  - Stackoverflow
---

    instance = SomeModel.objects.get(id=id)
    instance.delete()

    or

    SomeModel.objects.filter(id=id).delete()

    In the view file

    def user_data_remove(request, id):
        """Remove the user uploaded proteins individually"""

        instance = UserUploadData.objects.get(
            session_key=request.session.session_key, id=id)
        instance.delete()

    return redirect("view_cart")
