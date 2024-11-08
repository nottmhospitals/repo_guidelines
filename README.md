# User Code of Behaviour and Repository Guidelines for GitHub

## User Code of Behaviour

 - Registered users must belong to Nottingham University Hospitals NHS Trust or be approved external collaborators.
 - They must use their nhs.net email and  have set up a 2 factor authorisation. 
 - If users leave the organisation, or are inactive after 6 months, they will be converted to outside collaborator, and after 6 more months removed. 
 - Users will be respectful of other users and follow [code of conduct](https://github.com/nottmhospitals/user_and_repository_guidelines/blob/main/code_of_conduct.md) extracted from [here](https://github.com/nhs-r-community/NHSRdatasets/blob/main/CODE_OF_CONDUCT.md).

## Repository Guidelines

 - Repositories **must** be set to private until approved by an owner of the organisation repository.
 - The first **commit** must be the [.gitignore file included in this repository](https://github.com/nottmhospitals/user_and_repository_guidelines/blob/main/.gitignore) extracted from [here](https://github.com/Birmingham-and-Solihull-ICS/BSOLproject/blob/main/.gitignore)
 - Users **must** follow the [open code checklist](https://github.com/nottmhospitals/user_and_repository_guidelines/blob/main/Open%20Code%20Checklist.md) extracted from [here](https://github.com/nhsengland/github-WoW/blob/main/docs/Open_Code_Checklist.md)
 - In case of a data Breach, users **must** follow the [breach action steps](https://github.com/nottmhospitals/user_and_repository_guidelines/blob/main/Breach_Actions_Plan.md) extracted from [here](https://tools.nhsrcommunity.com/technical-git.html#removing-sensitive-and-patient-identifiable-information)
 - Parts of code containing business/analytical logic **must** be covered by unit tests to provide assurance that the code works in the way that it says it works
 - Code **must** be free of known malicious dependencies

Additionally, Here is a list of mandatory items to include in any organisation repositories (modified from [NHS england way of working](https://github.com/nhsengland/github-WoW)):

### Readme
Every repo should have a README which as a minimum specifies clearly the purpose of the repository.  Ideally this README file would be concise and include additional components covering ownership, development status, context, support for the user and how to contribute to the code. An ideal example readme can be seen [here](https://github.com/othneildrew/Best-README-Template/blob/master/BLANK_README.md)

### License
Every Repo should have an apporpiate associated license and copyright notice.  There are some cases when a license is not needed but this should be a thought through exception rather than the starting point.  The NHS Open Source Policy states: "NHS staff exert intellectual property rights for code and documentation through Crown Copyright. Using a copyright notice e.g. _Copyright (c) 2021 Crown Copyright_ ensures that rights to the relevant work reside with the UK Government, and that unless otherwise specified no-one else can copy, distribute or modify your work without risk. Licences then dictate further terms for how people may use copyrighted material.

**All open source projects must be accompanied by a licence.** The default option for NHS open source code is the widely permissive [MIT Licence](https://choosealicense.com/licenses/mit/). Your project may choose to use [APLv2](https://choosealicense.com/licenses/apache-2.0/) instead, and should consider doing so if your code is subject to regulatory requirements (see below). If you wish to ensure that no-one can make proprietary or closed source versions of your code, please use [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html). For all associated documentation you should use the [Open Government 3.0 Licence](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/): projects may use multiple licences for a project as long as they are explicit about which licence applies to which part of the project. Beyond licence assignment in a project’s README file, **the full text of the relevant licences should be included in a top level directory LICENCE file.**"

|Licence  |Use  |
|:---|:---|
| [MIT Licence](https://choosealicense.com/licenses/mit/) | Default licence for all new code  |
| [APLv2](https://choosealicense.com/licenses/apache-2.0) | Where code must be accompanied by legal notices  |
| [GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) | To prevent proprietary or closed re-use of code  |
| [Open Government 3.0 Licence](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) | Default licence for all documentation  |

### Changelog
A markdown file in your repository that tracks noteable changes to the code.  Recommendation is to use [semantic versioning](https://semver.org/spec/v2.0.0.html) which reflects `Breaking changes`, `New features`, and
`Fixes` clearly. 

### Contributing File
A piece of text that encourages contributions in the forms of raising new issues and submitting pull requests.  Include reference to the code of conduct and any guidance about branching strategy or style of commit messages to help contributions be made is a standardised way. 

### Model Card
When your code contains a piece of code which someone else may use or reproduce then it's best to make clear the intended use for the code and any known limitations.  One way to do this is to use a model card stating:
- model details 
- Intended use
- Out-of-scope usage
- Training data
- Performance and Limitations
- Notes to the user

### Templates For Pull Requests
to support contributions being submitted in a standardised form you can include a pull request template for fixes and new features.  This will then help contributors know what information to include to support these requests.

### Contact
Contact details in the README are useful but this often depends on an appropriate shared mailbox being avilable.

