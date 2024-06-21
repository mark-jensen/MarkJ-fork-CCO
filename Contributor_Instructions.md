### Branching:
`master` contain the latest release  
`develop` where pull requests are made from patch and feature branches  

### Instructions: 
- If you do not have write privileges in the repo, then create a fork and work off that. 
- All changes shall be made on an issue-specifc branch.
  - Use the feature in the isseu tracker located to the right under "Development" to create the branch. Make sure to "Change Branch Source" and select 'develop'.
- If the changes are not based on an existing issue, create one first, assign yourself.
- Make sure your preferred method of editing OWL files isn't generating spurious diffs.
  - To prevent this, make a token change to the file and save. E.g., add an annotation to the ontology "foo". Then use your favorite diff checker to confirm only that change is being rendered. Delete the change before making any other changes.
  - If you can't prevent the bogus diffs, then make a change to the file with a message "Change to render diffs correctly."
  - Delete the change and commit with message "Change for diffs deleted."
- Better to commit often rather than not enough. Ideally your commits will be have a unified objective. E.g., "changed language tags on all properties", "updated formatting for a few definitions", "deleted class Agent Identifier & fixed related axioms".
- Double check your work, make sure it loads in Protege, open All Core Ontology and confirm there are no bugs.
- Perform a PR on `develop`. Optionally, you may assign one or more reviewers, e.g., people that contributed to the issue. 

TODO: IRI schema, fork procedure
