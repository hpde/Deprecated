[![SPASE Manual Validation](https://github.com/hpde/Deprecated/actions/workflows/validate.yml/badge.svg)](https://github.com/hpde/Deprecated/actions/workflows/validate.yml)
[![SPASE Push Validation](https://github.com/hpde/Deprecated/actions/workflows/validate-push.yml/badge.svg)](https://github.com/hpde/Deprecated/actions/workflows/validate-push.yml)

# Deprecated
Resource descriptions that have been superseded.

# Validation Actions

GitHub actions are configured for this repository. When a "git push" occurs 
a validation and referential check is performed on the changes or additions 
to the repository since the last push. The status of the action is displayed in the
"SPASE Push Validation" badge at the top of the page. You can view the log of the
validation by viewing the [action workflows](../../actions), clicking on the appropriate workflow
run, then "validate-log" artifict.

The "SPASE Push Validation" is designed to incrementally validate the repository. It assumes
that the repository is valid before the "git push". To perform a whole repository validation
run the "SPASE Manual Validation" action.  To manually run an action go to the [actions](../../actions) page,
select the "SPASE Manual Validation" action, then click on "Run Workflow". For large repositories it 
can take many minutes for the workflow to complete - be patient. Once it is complete the "SPASE Manual Validation"
badge will update.

**Note on badge refresh**: The status portion of a badge is an image. Typically browsers cache images so an 
updated status may not appear immediately. One way to view the current badge is to clear cached images back to when you
last loaded the page.

**Notes for repository administrator**: There is no garbage collection for workflows. So, its a good practice to
occassionally visit the [action workflows](../../actions) and remove old workflow runs. To remove a run click
the elipses (...) for a work flow and select "Delete workflow run". Typically you would only need the most recent run.