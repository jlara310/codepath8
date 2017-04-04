# Project 7 - WordPress Pentesting

Time spent: **6** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

1. User Enumeration: Green site. If a user name exists, the error text is bold. If the error text is not bold, the user name does not exist
2. Indirect Object Reference: Red Site https://130.211.159.203/red/public/salesperson.php?id=11
3. SQLI: BLUE with https://130.211.159.203/blue/public/salesperson.php?id=1%27%20OR%20SLEEP(1)%23
4. Cross Site Scrpting: GREEN https://130.211.159.203/green/public/staff/feedback/index.php, feedback does not sanitize for javascript.
5. Cross Site Request Forgery: Red Site: https://130.211.159.203/red/public/staff/states/show.php?id=1 You can submit a form without a CSRF token. You can create form and trick and admin into submitting the form.
6. Session Hijacking/Fixation: Blue Site: https://130.211.159.203/blue/public/staff/feedback/index.php I copied PHPSESSID cookie from target browser to the attacking browser and was able to get into the admin area.

## Assets

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Describe any challenges encountered while doing the work

## License

    Copyright [2017] [Juan Lara]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.