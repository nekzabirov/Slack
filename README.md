# Slug plugin

**Plugin for send message to slack**

## Set up

1)  Copy **slack.gradle** to root of project
2)  Add `apply from: '../slack.gradle'` to **build.gradle**
3)  Add code bottom of app module **build.gradle**

    slack {  
      text = 'Vitau shanoviy kolegie.\n Ya opublikuvav onovlennya'  versionName = versionNameM  
      releaseNotes = releaseNotesM  
      task = taskName  
      webHooks = 'https://hooks.slack.com/services/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'  
      testerGroupName = testerGroup  
      developer = 'Nikita'  
    }

## Use

    ./gradlew sendSlack

