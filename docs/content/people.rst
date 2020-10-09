===============
People/Profiles
===============

Each individual should have their own markdown file representing their profile.
These markdown files should be placed under the :code:`_people` directory under
the root of the repository. Each profile also has a thumbnail image file that
will be referenced in the markdown file. These image files should be placed
under the :code:`images/people` directory under the root of the repository.

.. _naming-convention:

The naming convention of the files should follow the standard of all lowercase
with underscores between the first and last name of the person, e.g.
:code:`first_last.md`.

Modifying A Profile
===================

All profiles are defined by three things, split between two files.

#. :ref:`content/people:the header`

#. :ref:`content/people:the bio`

#. :ref:`content/people:profile thumbnail`

The header and bio are contained in a markdown file, while a jpg file is used
as the profile thumbnail.

Below is the content of the template profile as markdown.

.. literalinclude:: ../../_people/profile_template.md
    :language: text
    :linenos:
    :caption: Profile Template (:code:`_people/profile_template.md`)

The Header
----------

The header, line 1-14 of the above file, contains several variables that are
used to autogenerate a profile. This file provides all variables a profile can
use. The variables :term:`name`, :term:`avatar`, :term:`position`,
:term:`permalink` and :term:`title` are required. The other variables will be
ignored if left empty. However, it is highly recommended to fill out as many of
these variables as you can. This will improve the profile significantly.

.. glossary::

    name : String
        First and last name of the individual.

    degree : String (optional)
        The highest degree held, the concentration of the degree and followed
        by the university where obtained.

    position : pre-defined
        Choose one of the provided options, based on the role of the
        individual.

    focus : String (optional)
        A concentration or focus of your research.

    hours : String (optional)
        Generally reserved for postdoc and researchers. You can choose your
        preference in formatting here, e.g. "9:00AM - 5:00PM", "0900 - 1700",
        etc.

    location : String (optional)
        Where the individual sits when at Stanford. MSL room is Durand 028.

    email : String (optional)
        The email for the individual.

    projects : List (optional)
        A collection of projects the individual worked on. Please see
        _`project options` for the available projects.

    avatar : filename
        The filename of the image for the profile thumbnail. This file should
        be under the :code:`images/people` directory and should follow the
        :ref:`naming convention <naming-convention>`, with '.jpg' extension.

    permalink : website location
        The location of the profile with respect to the root website address.
        This should follow the :ref:`naming convention <naming-convention>`,
        e.g. /first_last/.

    title : String
        Same as the name variable. This is what will be the title of the tab in
        the browser.

    website : web address
        If the individual has an external website they would like to add to
        their profile.

.. todo::

    Need to create and then link the project options to the page related to
    which project names are available. Should use the label project-options and
    use the :ref: directive.

The Bio
-------

The bio is a section under the header that is used as a short bio for the
individual. This should be a short description of the person, including their
goals while working in the MSL.

Profile Thumbnail
-----------------

The profile thumbnail should be a square JPEG of the person. Preferably a
head shot of the individual. The image should be no larger than 800 x 800
pixels. The largest an image will ever become in the generated website pages
will be 500 pixel. As this might change in the future the 800 pixel value is
ideal in case things change, while minimizing storage space.

Once again, this file should be stored in the :code:`images/people` directory
of the repository root and follow the
:ref:`naming convention <naming-convention>` discussed above, with
:code:`.jpg` as the extension type.
    

Adding A New Person
===================

The easiest way to add a new individual is to copy the
:code:`_people/profile_template.md` and rename it to match the person being
added. Once the file is added to the :code:`_people` directory, the website
should automatically create the profile page. Just make sure you follow the
procedures in `Modifying A Profile`_ to update the template information.