=====
Posts
=====

Posts is a simple Django app to conduct Web-based blog. For each
blog you can see it and like and comment as well.

Detailed documentation is in the "docs" directory.

Quick start
-----------

1. Add "posts" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'posts',
    ]

2. Include the posts URLconf in your project urls.py like this::

    url(r'^posts/', include('posts.urls')),

3. Run `python manage.py migrate` to create the posts models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a posts (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/posts/ to participate in the posts.
