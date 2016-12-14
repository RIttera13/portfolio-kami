---
layout: post
title: Blocipedia
thumbnail-path: "img/blocipedia.png"
short-description: Wikis, It's a place for sharing knowledge.

---

{:.center}
![]({{ site.baseurl }}/img/blocipedia.png)

## Explanation

Blocipedia is a basic Wikipedia style site. It uses a number of features and functions that help make a good collaborative Wiki app. This is a project included in the Bloc program. It gives a list of user stories and some guidance throughout, but I (the student) had to figure out how to accomplish each goal.

## Problem

The main features of this app include:

User Creation/Login/Password Recovery -

	This was accomplished using the _devise_ gem and incorporating its forms with some customization.


User roles -

	_pundit_ gem was used to establish policies and roles are defined to include Standard/Premium/Admin.

	* A guest (not logged in), can access the site and view the wikis that are set to public.

	* A Standard user is a free account that can create public wikis, edit/delete their own wikis, and  can be set as a collaborator on other wikis to allow them editing privileges.

	* A Premium user is a one time paid account ($15). It can create public/private wikis, edit/delete that users wikis, add collaborators to their wikis to give any chosen member edit privileges.

	* Admin users have full control. These are rare entities, and no members are given this role.


Wiki CRUD -

  The ability to create/edit/update/destroy wikis is crucial in a wiki app. The database keeps track of the wikis. It associates them with the users that created them, and it also associates the wikis with any users designated as collaborators.

Collaborators -

	These are other members that have been granted permission to edit wikis that do not	belong to them. Collaborators can only be changed by the owner of the wiki (premium users only) or an admin. Any member (including Standard users) are allowed to be collaborators on a wiki, even those designated as private.

## Results

This was a fun and tricky exercise. It has a lot of new pieces I had not been introduces to before. It had enough to be challenging, while also not being over whelming. It allowed me to put some fun personal changes in and I am happy with the results.
