[![Maven](https://img.shields.io/maven-central/v/{{.Gitstrap.Params.package}}/{{.Repo.Name}}.svg)](https://mvnrepository.com/artifact/{{.Gitstrap.Params.package}}/{{.Repo.Name}})
[![Javadocs](http://www.javadoc.io/badge/{{.Gitstrap.Params.package}}/{{.Repo.Name}}.svg)](http://www.javadoc.io/doc/{{.Gitstrap.Params.package}}/{{.Repo.Name}})
[![License: MIT](https://img.shields.io/github/license/mashape/apistatus.svg)](./license.txt)
[![Commit activity](https://img.shields.io/github/commit-activity/y/{{.Repo.Owner.Login}}/{{.Repo.Name}}.svg?style=flat-square)](https://github.com/{{.Repo.Owner.Login}}/{{.Repo.Name}}/graphs/commit-activity)

[![Build Status](https://circleci.com/gh/{{.Repo.Owner.Login}}/{{.Repo.Name}}.svg?style=svg)](https://circleci.com/gh/{{.Repo.Owner.Login}}/{{.Repo.Name}})
[![0pdd](http://www.0pdd.com/svg?name={{.Repo.Owner.Login}}/{{.Repo.Name}})](http://www.0pdd.com/p?name={{.Repo.Owner.Login}}/{{.Repo.Name}})
[![Dependency Status](https://requires.io/github/{{.Repo.Owner.Login}}/{{.Repo.Name}}/requirements.svg?branch=master)](https://requires.io/github/{{.Repo.Owner.Login}}/{{.Repo.Name}}/requirements/?branch=master)
[![Known Vulnerabilities](https://snyk.io/test/github/{{.Repo.Owner.Login}}/{{.Repo.Name}}/badge.svg)](https://snyk.io/org/{{.Repo.Owner.Login}}/project/3bd606b4-323a-4a5e-a9cf-8fe847b7f94d/?tab=dependencies&vulns=vulnerable)

[![DevOps By Rultor.com](http://www.rultor.com/b/{{.Repo.Owner.Login}}/{{.Repo.Name}})](http://www.rultor.com/p/{{.Repo.Owner.Login}}/{{.Repo.Name}})
[![EO badge](http://www.elegantobjects.org/badge.svg)](http://www.elegantobjects.org/#principles)
[![We recommend IntelliJ IDEA](http://www.elegantobjects.org/intellij-idea.svg)](https://www.jetbrains.com/idea/)

[![Qulice](https://img.shields.io/badge/qulice-passed-blue.svg)](http://www.qulice.com/)
[![SQ maintainability](https://sonarcloud.io/api/project_badges/measure?project={{.Gitstrap.Params.package}}%3A{{.Repo.Name}}&metric=sqale_rating)](https://sonarcloud.io/dashboard?id={{.Gitstrap.Params.package}}%3A{{.Repo.Name}})
[![Codebeat](https://codebeat.co/badges/03a70479-61fe-4167-bf43-84dfd78d4cc0)](https://codebeat.co/projects/github-com-{{.Repo.Owner.Login}}-{{.Repo.Name}}-master)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/e72eb423424b4b6db9ba64aa97463206)](https://www.codacy.com/app/{{.Repo.Owner.Login}}/{{.Repo.Name}}?utm_source=github.com&amp;utm_medium=referral&amp;utm_content={{.Repo.Owner.Login}}/{{.Repo.Name}}&amp;utm_campaign=Badge_Grade)
[![Codecov](https://codecov.io/gh/{{.Repo.Owner.Login}}/{{.Repo.Name}}/branch/master/graph/badge.svg)](https://codecov.io/gh/{{.Repo.Owner.Login}}/{{.Repo.Name}})

## What it is
{{.Repo.Description}}

## Principles
[Design principles](http://www.elegantobjects.org#principles) behind {{.Repo.Name}}.

## How to use
Get the latest version [here](https://github.com/{{.Repo.Owner.Login}}/{{.Repo.Name}}/releases):

```xml
<dependency>
    <groupId>{{.Gitstrap.Params.package}}</groupId>
    <artifactId>{{.Repo.Name}}</artifactId>
    <version>${version}</version>
</dependency>
```

Java version required: 1.8+.

Interface           | Purpose                                               | Implementations / Related                    
--------------------|-------------------------------------------------------|---------------------------
[Inbox](#inbox)     | Allows to read the emails from the server             | [JavaxMailInbox](src/main/java/io/github/dgroup/mbox4j/inbox/javax/JavaxMailInbox.java), [InboxEnvelope](src/main/java/io/github/dgroup/mbox4j/inbox/InboxEnvelope.java), [UncheckedInbox](src/main/java/io/github/dgroup/mbox4j/inbox/UncheckedInbox.java), [FakeInbox](src/main/java/io/github/dgroup/mbox4j/inbox/FakeInbox.java), [etc](src/main/java/io/github/dgroup/mbox4j/inbox)                            

All examples below are using the following frameworks/libs:
 - [Hamcrest](https://github.com/hamcrest/JavaHamcrest) - Library of matchers, which can be combined in to create flexible expressions of intent in tests.
 - [cactoos](https://github.com/yegor256/cactoos) - Object-Oriented Java primitives, as an alternative to Google Guava and Apache Commons.
 - [cactoos-matchers](https://github.com/yegor256/cactoos) - Object-Oriented Hamcrest matchers

### [Inbox](src/main/java/io/github/dgroup/mbox4j/Inbox.java)

{{if .Gitstrap.Params.readmeContrib}}
## Contribution
{{.Gitstrap.Params.readmeContrib}}
{{end}}
