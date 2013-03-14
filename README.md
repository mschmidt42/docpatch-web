#   DocPatch Website


##  Deployment

Clone this repository and fetch all sub modules:

    git clone git@gitlab.die-foobar.de:benjamin/docpatch-web.git
    git submodule init
    git submodule update

Build the repository and create output files:

    cd grundgesetz-dev/
    docpatch build
    docpatch create -t -r all -f pdf
    docpatch create -t -r all -f html
    docpatch create -t -r all -f plain
    docpatch create -t -r all -f odt
    docpatch create -t -r all -f epub

These output formats are just examples. Type `docpatch create --help` for more information.

Edit the Kickstrap configuration file `kickstrap.less` and adapt the root directory to your needs.

Upload everything and have fun! :-)


##  ToDo

*   Historie einzelner Artikel betrachten
*   Anderes Wort für "Revision" => "Fassung"?
*   Vergleich:
    *   "alte" und "neue" Revision
    *   Nur Änderungen anzeigen; gesamter Text ist verwirrend zu viel
*   Herunterladen
    *   Zu lange Titel
    *   Datum präsenter anzeigen, weil wichtig
    *   Tooltips nutzen
*   Layout
    *   Anker-Offset setzen
    *   scrollTo() funktioniert nicht
