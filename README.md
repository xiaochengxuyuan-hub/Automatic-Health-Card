# Health Info Auto Report (SUES)

A script that helps you fill out the health report automatically at a set time.

## Usage

**CAUTION: Please fill out the report manually in [report website](my.sues.edu.cn) before using this tool.**

We recommend you try the remote environment: Github Actions

1. Fork this repo to your own repositories.
2. Add repository secrets in the sheet by click `Settings` >>> `Secrets`(left sidebar)>>>`New repository secret
` in your forked repo:
   
    | Name      | Val | example|
    | ----------- | ----------- | ----------- |
    | NUM   | your student ID    |011383246|
    | PWD   | password           |*********|
    | MAIL  | Notice mail address|011383246@sues.edu.cn|

    - Free free to add those values that only you can see them.
    - [Click here to see how to add secerts](https://docs.github.com/en/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository)
    - Connect with your school email (@sues.edu.cn) on your Wechat
      to get mail notifications.
      
      
## Configuration

change the following codes in `.github/workflows` >>> `python-app.yml` to schedule action time

      schedule:
        - cron: '31 22 * * *'
        - cron: '12 0 * * *'
        - cron: '48 2 * * *'
        - cron: '6 6 * * *'
        - cron: '36 8 * * *'
        - cron: '54 10 * * *'


__Remark: '31 22 * * *' - - run daily at 22:31(UTC time)-- 6:31(UTC+8 Beijing, China Time)__

## Contributor
This tool exists thanks to all the people who contribute.

[__@HynemanKan__](https://github.com/HynemanKan)

[__@zsqw123__](https://github.com/zsqw123)

