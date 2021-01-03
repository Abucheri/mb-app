# This small message board app is based on William Vincent's book django for beginners
We will start by making our model to hold messages entered bu users.
open posts/models.py to do this.
now create your migrations to accomodate our model.
set up the admin by creating the site superuser.
we need to register our model in posts/admin.py for us to manage it via the admin interface.
let's create some posts objects using the admin.
now we want to list our contents using generic class-based ListView.
let's go to posts/views.py.
lets add our project level templates folder and register in settings.py.
since we want to return a list of objects, we'll use 'object_list' name since this is the variable returned by ListView.
object_list leads to confusion sometimes, so we are going to change the context_object_name in posts/views.py.
also update our template.
Let's set up our urls starting with the project level urls then our app urls.
now let's do the app testing using the model.
now we neeed to test our view, we will add one more test for the view to test if it exists.
We’ll add one more import at the top for reverse and a brand new class HomePageViewTest for our test