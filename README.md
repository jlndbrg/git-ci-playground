# git-ci-playground

Conventional commits används för merga av PRs och commits som ska räknas upp i release notes och ligga till grund för semversion av releasetag. 

Använder semantic-release för att 
- skapa upp semantiskt versionerad release tag 
- automatiska sammanställa release notes utifrån conventional commits

 "releaseRules": [
            { "type": "feat", "release": "minor" },
            { "type": "fix", "release": "patch" },
            { "type": "docs", "release": "patch" },
            { "type": "style", "release": "patch" },
            { "type": "refactor", "release": "patch" },
            { "type": "perf", "release": "patch" },
            { "type": "test", "release": "patch" },
            { "type": "chore", "release": false },
            { "type": "build", "release": false },
            { "type": "ci", "release": false }
          ],
          "parserOpts": {
            "noteKeywords": ["BREAKING CHANGE", "BREAKING CHANGES"]
          }