git-generate-changelog(1) - Generate changelog from github
================================

## SYNOPSIS

`git generate-changelog` [-h|--help] [-u|--user] [-p|--project]

## DESCRIPTION

Automatically generate change log from your tags, issues, labels and pull requests on GitHub.

## OPTIONS

  -u, --user [USER]

  Username of the owner of target GitHub repo

  -p, --project [PROJECT]

  Name of project on GitHub

  -t, --token [TOKEN]

  To make more than 50 requests per hour your GitHub token is required. You can generate it at: https://github.com/settings/tokens/new

  -f, --date-format [FORMAT]

  Date format. Default is %Y-%m-%d

  -o, --output [NAME]

  Output file. Default is CHANGELOG.md

  -b, --base [NAME]

  Optional base file to append generated changes to.

   --bugs-label [LABEL]

   Setup custom label for bug-fixes section. Default is "**Fixed bugs:**

   --enhancement-label [LABEL]

   Setup custom label for enhancements section. Default is "**Implemented enhancements:**"

   --issues-label [LABEL]

   Setup custom label for closed-issues section. Default is "**Closed issues:**"

   --header-label [LABEL]

   Setup custom header label. Default is "# Change Log"

   --pr-label [LABEL]

   Setup custom label for pull requests section. Default is "**Merged pull requests:**"

   --[no-]issues

   Include closed issues in changelog. Default is true

   --[no-]issues-wo-labels

   Include closed issues without labels in changelog. Default is true

   --[no-]pr-wo-labels

   Include pull requests without labels in changelog. Default is true

   --[no-]pull-requests

   Include pull-requests in changelog. Default is true

   --[no-]filter-by-milestone

   Use milestone to detect when issue was resolved. Default is true

   --[no-]author

   Add author of pull-request in the end. Default is true

   --unreleased-only

   Generate log from unreleased closed issues only.

   --[no-]unreleased

   Add to log unreleased closed issues. Default is true

   --unreleased-label [label]

   Add to log unreleased closed issues. Default is true

   --[no-]compare-link

   Include compare link (Full Changelog) between older version and newer version. Default is true

   --include-labels x,y,z

   Only issues with the specified labels will be included in the changelog.

   --exclude-labels x,y,z

   Issues with the specified labels will be always excluded from changelog. Default is 'duplicate,question,invalid,wontfix'

   --bug-labels x,y,z

   Issues with the specified labels will be always added to "Fixed bugs" section. Default is 'bug,Bug'

   --enhancement-labels x,y,z

   Issues with the specified labels will be always added to "Implemented enhancements" section. Default is 'enhancement,Enhancement'

   --between-tags x,y,z

   Change log will be filled only between specified tags

   --exclude-tags x,y,z

   Change log will exclude specified tags

   --since-tag x

   Change log will start after specified tag

   --due-tag x

   Change log will end before specified tag

   --max-issues [NUMBER]

   Max number of issues to fetch from GitHub. Default is unlimited

   --release-url [URL]

   The URL to point to for release links, in printf format (with the tag as variable).

   --github-site [URL]

   The Enterprise Github site on which your project is hosted.

   --github-api [URL]

   The enterprise endpoint to use for your Github API.

   --simple-list

   Create simple list from issues and pull requests. Default is false.

   --future-release [RELEASE-VERSION]

   Put the unreleased changes in the specified release number.

   --[no-]verbose

   Run verbosely. Default is true

  -v, --version

  Print version number

  -h, --help

  Displays Help


## EXAMPLES

## AUTHOR

Written by Petr Korolev sky4winder@gmail.com

## REPORTING BUGS

&lt;<https://github.com/skywinder/github-changelog-generator/issues>&gt;

## SEE ALSO

&lt;<https://github.com/skywinder/github-changelog-generator/>&gt;
