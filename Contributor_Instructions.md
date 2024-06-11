### Branching:
`master` contain the latest release
`develop` where pull requests are made from patch and feature branches

### Instructions:

- All changes shall be made on a patch/feature branch that is created from an issue. Use the feature located to the right under Development to create branch. Make sure to select "Change Branch Source" and select 'develop'.
If the changes are not based on an existing issue, create one.
Make sure your preferred method of editing OWL files isn't generating spurious diffs. To prevent this, make a token change (e.g., add an annotation to the ontology) to the file and save it.
Then use your favorite diff checker to confirm only that change is being rendered. Different versions of OWL API and Protégé will sometimes cause formatting issues.
If you can't prevent the bogus diffs, then make commit the file with a message "Bogus change to render diffs correctly".
Better to commit often rather than not enough. Ideally your commits will be have a unified objective. E.g., "changed language tags on all properties", "updated formatting for a few definitions", "deleted class Agent Identifier & fixed related axioms".
When you've made changes as dictated by the issue, then perform a MR on develop.
