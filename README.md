Liquibase exercise


Verify changelog

 liquibase --changeLogFile=changelog.h2.sql updateSQL


 Deploy change

 liquibase --changeLogFile=changelog.h2.sql update


Generate changelog
liquibase --changeLogFile=generatedchangelog.h2.sql generateChangelog
liquibase --changeLogFile=generatedchangelog.h2.xml generateChangelog


Rollback change

liquibase --changelog-file=changelog.h2.sql rollback-count 1


Build a snapshot

liquibase --outputFile=myschemaSnapshot.yaml snapshot --snapshotFormat=yaml


Diff

liquibase --outputFile=mydiff.txt diff


liquibase rollback --

mvn liquibase:update

mvn liquibase:rollback

mvn liquibase:rollback -Dliquibase.rollbackCount=1

