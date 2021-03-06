History
-------

0.1.0 (2017-09-25)
++++++++++++++++++

* Initial release

0.1.2 (2017-09-26)
++++++++++++++++++

* Merge Quickstart section into README

0.1.3 (2017-09-26)
++++++++++++++++++

* Add missing HISTORY.rst to manifst

0.1.4 (2017-09-26)
++++++++++++++++++

* Support for ``order_field`` attribute for ``list_display`` method fields.
  This works similar to ``ModelAdmin`` method fields' ``admin_order_field``
  property.

0.1.5 (2017-09-26)
++++++++++++++++++

* Better unicode support

0.1.6 (2017-09-27)
++++++++++++++++++

* Better access control support through 'login_url' & 'raise_exception'
  PopupCrudViewSet properties

0.1.7 (2017-10-13)
++++++++++++++++++

* Object detail view support 

0.1.8 (2017-10-16)
++++++++++++++++++

* Add PopupCrudViewSet.urls() -- a single method to return all the CRUD urls 
  that can be added to urlpatterns[].
* When related object popup is activated on a multiselect select and it adds a 
  new object, the object is added to the existing list of selections. (old code
  used to replace all the current selections with the newly added item)
* Insert all form media into ListView through ListView.media property. 
* Fix broken support for django-select2 in modals by setting control's 
  dropdownParent to the modal (rather than parent window)
* Use the 'create-edit-modal' modal as the template for secondary modals
  activated through related-model modal popups. This ensures consistent modal 
  look and feel if the user customized the modal template by overriding 
  popupcrud/modal.html template.
* Fix ALLOWED_HOSTS in settings - issue #1

0.2.0 (2017-10-18)
++++++++++++++++++
* Bumping minor version as reflection of new features legacy_crud dict, media 
  & out-of-the-box django_select2 support in previous release
* Added 'crudform.ready' JavaScript event, which is triggered when 
  create/update form is activated. This event provides clients an uniform way to 
  apply their own optional initialization code to the CRUD forms.
* Added 6 more tests to cover new legacy_crud dict value support & form media
  injection.
