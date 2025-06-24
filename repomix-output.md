This file is a merged representation of the entire codebase, combined into a single document by Repomix.

# File Summary

## Purpose
This file contains a packed representation of the entire repository's contents.
It is designed to be easily consumable by AI systems for analysis, code review,
or other automated processes.

## File Format
The content is organized as follows:
1. This summary section
2. Repository information
3. Directory structure
4. Multiple file entries, each consisting of:
  a. A header with the file path (## File: path/to/file)
  b. The full contents of the file in a code block

## Usage Guidelines
- This file should be treated as read-only. Any changes should be made to the
  original repository files, not this packed version.
- When processing this file, use the file path to distinguish
  between different files in the repository.
- Be aware that this file may contain sensitive information. Handle it with
  the same level of security as you would the original repository.

## Notes
- Some files may have been excluded based on .gitignore rules and Repomix's configuration
- Binary files are not included in this packed representation. Please refer to the Repository Structure section for a complete list of file paths, including binary files
- Files matching patterns in .gitignore are excluded
- Files matching default ignore patterns are excluded
- Files are sorted by Git change count (files with more changes are at the bottom)

## Additional Info

# Directory Structure
```
.repomixignore
BackEnd/.git/config
BackEnd/.git/description
BackEnd/.git/FETCH_HEAD
BackEnd/.git/HEAD
BackEnd/.git/hooks/applypatch-msg.sample
BackEnd/.git/hooks/commit-msg.sample
BackEnd/.git/hooks/fsmonitor-watchman.sample
BackEnd/.git/hooks/post-update.sample
BackEnd/.git/hooks/pre-applypatch.sample
BackEnd/.git/hooks/pre-commit.sample
BackEnd/.git/hooks/pre-merge-commit.sample
BackEnd/.git/hooks/pre-push.sample
BackEnd/.git/hooks/pre-rebase.sample
BackEnd/.git/hooks/pre-receive.sample
BackEnd/.git/hooks/prepare-commit-msg.sample
BackEnd/.git/hooks/push-to-checkout.sample
BackEnd/.git/hooks/sendemail-validate.sample
BackEnd/.git/hooks/update.sample
BackEnd/.git/info/exclude
BackEnd/.git/logs/HEAD
BackEnd/.git/logs/refs/heads/main
BackEnd/.git/logs/refs/remotes/origin/HEAD
BackEnd/.git/packed-refs
BackEnd/.git/refs/heads/main
BackEnd/.git/refs/remotes/origin/HEAD
BackEnd/.gitignore
BackEnd/index.js
BackEnd/middleware/authMiddleware.js
BackEnd/middleware/decryptionMiddleware.js
BackEnd/middleware/firebaseAdminMiddleware.js
BackEnd/middleware/oauthTokenMiddleware.js
BackEnd/middleware/roleBasedDataMiddleware.js
BackEnd/middleware/uploadFileMiddleware.js
BackEnd/middleware/uploadMiddleware.js
BackEnd/package.json
BackEnd/prisma/migrations/20250201195516_init/migration.sql
BackEnd/prisma/migrations/20250201200911_change_ids_to_int/migration.sql
BackEnd/prisma/migrations/20250203162645_add_user_business_models/migration.sql
BackEnd/prisma/migrations/20250203185734_changed/migration.sql
BackEnd/prisma/migrations/20250203190329_added/migration.sql
BackEnd/prisma/migrations/20250206183710_added/migration.sql
BackEnd/prisma/migrations/20250207191540_added/migration.sql
BackEnd/prisma/migrations/20250209223549_removed/migration.sql
BackEnd/prisma/migrations/20250210232144_added/migration.sql
BackEnd/prisma/migrations/20250214023231_replaced/migration.sql
BackEnd/prisma/migrations/20250214234943_updated/migration.sql
BackEnd/prisma/migrations/20250304180920_updated/migration.sql
BackEnd/prisma/migrations/20250310210628_removed/migration.sql
BackEnd/prisma/migrations/20250311153000_adjusted/migration.sql
BackEnd/prisma/migrations/20250314193459_adjusted/migration.sql
BackEnd/prisma/migrations/20250322164348_created/migration.sql
BackEnd/prisma/migrations/20250322171321_updated/migration.sql
BackEnd/prisma/migrations/20250322193650_updated/migration.sql
BackEnd/prisma/migrations/20250322201228_updated/migration.sql
BackEnd/prisma/migrations/20250401163908_favourite/migration.sql
BackEnd/prisma/migrations/migration_lock.toml
BackEnd/prisma/schema.prisma
BackEnd/prisma/seed.js
BackEnd/README.md
BackEnd/routes/admin/adminStatsRoute.js
BackEnd/routes/admin/userDetailsRoute.js
BackEnd/routes/admin/verifyUserRoute.js
BackEnd/routes/appointment.js
BackEnd/routes/authRoutes.js
BackEnd/routes/availabilityRoutes.js
BackEnd/routes/calendarAuthRoutes.js
BackEnd/routes/carListingRoutes.js
BackEnd/routes/consultantRoutes.js
BackEnd/routes/dashboardRoutes.js
BackEnd/routes/houseListingRoutes.js
BackEnd/routes/onboardingRoutes.js
BackEnd/testIframe.html
Frontend/.git/config
Frontend/.git/description
Frontend/.git/FETCH_HEAD
Frontend/.git/HEAD
Frontend/.git/hooks/applypatch-msg.sample
Frontend/.git/hooks/commit-msg.sample
Frontend/.git/hooks/fsmonitor-watchman.sample
Frontend/.git/hooks/post-update.sample
Frontend/.git/hooks/pre-applypatch.sample
Frontend/.git/hooks/pre-commit.sample
Frontend/.git/hooks/pre-merge-commit.sample
Frontend/.git/hooks/pre-push.sample
Frontend/.git/hooks/pre-rebase.sample
Frontend/.git/hooks/pre-receive.sample
Frontend/.git/hooks/prepare-commit-msg.sample
Frontend/.git/hooks/push-to-checkout.sample
Frontend/.git/hooks/sendemail-validate.sample
Frontend/.git/hooks/update.sample
Frontend/.git/info/exclude
Frontend/.git/logs/HEAD
Frontend/.git/logs/refs/heads/main
Frontend/.git/logs/refs/remotes/origin/HEAD
Frontend/.git/packed-refs
Frontend/.git/refs/heads/main
Frontend/.git/refs/remotes/origin/HEAD
Frontend/.gitignore
Frontend/components.json
Frontend/eslint.config.mjs
Frontend/next.config.ts
Frontend/package.json
Frontend/postcss.config.mjs
Frontend/README.md
Frontend/src/app/(auth)/forgot-password/page.tsx
Frontend/src/app/(auth)/layout.tsx
Frontend/src/app/(auth)/login/page.tsx
Frontend/src/app/(auth)/onboarding/car-dealer/BusinessInformation.tsx
Frontend/src/app/(auth)/onboarding/car-dealer/page.tsx
Frontend/src/app/(auth)/onboarding/car-dealer/SuccessPage.tsx
Frontend/src/app/(auth)/onboarding/car-dealer/types.ts
Frontend/src/app/(auth)/onboarding/consultant/BusinessInformation.tsx
Frontend/src/app/(auth)/onboarding/consultant/page.tsx
Frontend/src/app/(auth)/onboarding/consultant/SuccessPage.tsx
Frontend/src/app/(auth)/onboarding/consultant/types.ts
Frontend/src/app/(auth)/onboarding/immigrant/page.tsx
Frontend/src/app/(auth)/onboarding/layout.tsx
Frontend/src/app/(auth)/onboarding/page.tsx
Frontend/src/app/(auth)/onboarding/realtor/BusinessInformation.tsx
Frontend/src/app/(auth)/onboarding/realtor/OfficeWorkSetup.tsx
Frontend/src/app/(auth)/onboarding/realtor/page.tsx
Frontend/src/app/(auth)/onboarding/realtor/SuccessPage.tsx
Frontend/src/app/(auth)/onboarding/realtor/types.ts
Frontend/src/app/(auth)/signup/page.tsx
Frontend/src/app/dashboard/admin/page.tsx
Frontend/src/app/dashboard/admin/user-list/page.tsx
Frontend/src/app/dashboard/admin/verify-users/page.tsx
Frontend/src/app/dashboard/admin/view-user/[id]/page.tsx
Frontend/src/app/dashboard/car-dealer/add-listing/page.tsx
Frontend/src/app/dashboard/car-dealer/availability/page.tsx
Frontend/src/app/dashboard/car-dealer/bookings/page.tsx
Frontend/src/app/dashboard/car-dealer/car-listings/[id]/page.tsx
Frontend/src/app/dashboard/car-dealer/car-listings/page.tsx
Frontend/src/app/dashboard/car-dealer/edit-listing/[id]/page.tsx
Frontend/src/app/dashboard/car-dealer/page.tsx
Frontend/src/app/dashboard/consultant/availability/page.tsx
Frontend/src/app/dashboard/consultant/bookings/page.tsx
Frontend/src/app/dashboard/consultant/page.tsx
Frontend/src/app/dashboard/layout.tsx
Frontend/src/app/dashboard/not-verified/page.tsx
Frontend/src/app/dashboard/page.tsx
Frontend/src/app/dashboard/realtor/add-listing/page.tsx
Frontend/src/app/dashboard/realtor/availability/page.tsx
Frontend/src/app/dashboard/realtor/bookings/page.tsx
Frontend/src/app/dashboard/realtor/edit-listing/[id]/page.tsx
Frontend/src/app/dashboard/realtor/house-listings/[id]/page.tsx
Frontend/src/app/dashboard/realtor/house-listings/page.tsx
Frontend/src/app/dashboard/realtor/page.tsx
Frontend/src/app/dashboard/user/bookings/page.tsx
Frontend/src/app/dashboard/user/cars/car-listings/[id]/page.tsx
Frontend/src/app/dashboard/user/cars/page.tsx
Frontend/src/app/dashboard/user/consultant/page.tsx
Frontend/src/app/dashboard/user/favourites-car/page.tsx
Frontend/src/app/dashboard/user/favourites-house/page.tsx
Frontend/src/app/dashboard/user/homes/house-listings/[id]/page.tsx
Frontend/src/app/dashboard/user/homes/page.tsx
Frontend/src/app/dashboard/user/page.tsx
Frontend/src/app/dashboard/user/profile/page.tsx
Frontend/src/app/dashboard/user/saved/page.tsx
Frontend/src/app/dashboard/user/slots/[listingId]/[type]/page.tsx
Frontend/src/app/dashboard/user/slots/consultant/[consultantId]/page.tsx
Frontend/src/app/globals.css
Frontend/src/app/layout.tsx
Frontend/src/app/page.tsx
Frontend/src/components/availability/AppointmentBooking.tsx
Frontend/src/components/availability/AvailabilityForm.tsx
Frontend/src/components/availability/AvailabilityPage.tsx
Frontend/src/components/availability/BookingTable.tsx
Frontend/src/components/availability/UserBooking.tsx
Frontend/src/components/consultant/ConsultantCarousel.tsx
Frontend/src/components/consultant/UpcomingMeetings.tsx
Frontend/src/components/Filter.tsx
Frontend/src/components/Footer.tsx
Frontend/src/components/Header.tsx
Frontend/src/components/ListingCard.tsx
Frontend/src/components/Listings.tsx
Frontend/src/components/Logo.tsx
Frontend/src/components/onboarding/DocumentUpload.tsx
Frontend/src/components/onboarding/PersonalInformation.tsx
Frontend/src/components/onboarding/TermsAndConditions.tsx
Frontend/src/components/providers/theme-provider.tsx
Frontend/src/components/QuickLinks.tsx
Frontend/src/components/Sidecard.tsx
Frontend/src/components/ThemeSwitcher.tsx
Frontend/src/components/ui/alert.tsx
Frontend/src/components/ui/button.tsx
Frontend/src/components/ui/calendar.tsx
Frontend/src/components/ui/card.tsx
Frontend/src/components/ui/chart.tsx
Frontend/src/components/ui/checkbox.tsx
Frontend/src/components/ui/dialog.tsx
Frontend/src/components/ui/dropdown-menu.tsx
Frontend/src/components/ui/form.tsx
Frontend/src/components/ui/input.tsx
Frontend/src/components/ui/label.tsx
Frontend/src/components/ui/popover.tsx
Frontend/src/components/ui/radio-group.tsx
Frontend/src/components/ui/scroll-area.tsx
Frontend/src/components/ui/select.tsx
Frontend/src/components/ui/table.tsx
Frontend/src/components/ui/tabs.tsx
Frontend/src/components/ui/textarea.tsx
Frontend/src/components/ui/toast.tsx
Frontend/src/components/ui/toaster.tsx
Frontend/src/components/UserProfile.tsx
Frontend/src/hooks/use-toast.ts
Frontend/src/lib/auth.ts
Frontend/src/lib/utils.ts
Frontend/src/middleware.ts
Frontend/tailwind.config.ts
Frontend/tsconfig.json
repomix.config.json
```

# Files

## File: .repomixignore
````
# Add patterns to ignore here, one per line
# Example:
# *.log
# tmp/

node_modules
````

## File: BackEnd/.git/config
````
[core]
	repositoryformatversion = 0
	filemode = false
	bare = false
	logallrefupdates = true
	symlinks = false
	ignorecase = true
[remote "origin"]
	url = https://github.com/rajatsachdeva31/ImmiGrowAI-BackEnd.git
	fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
	remote = origin
	merge = refs/heads/main
	vscode-merge-base = origin/main
````

## File: BackEnd/.git/description
````
Unnamed repository; edit this file 'description' to name the repository.
````

## File: BackEnd/.git/FETCH_HEAD
````
6e7d2815f0e46bf3b7a82dffdd9929d48f8bd540		branch 'main' of https://github.com/rajatsachdeva31/ImmiGrowAI-BackEnd
````

## File: BackEnd/.git/HEAD
````
ref: refs/heads/main
````

## File: BackEnd/.git/hooks/applypatch-msg.sample
````
#!/bin/sh
#
# An example hook script to check the commit log message taken by
# applypatch from an e-mail message.
#
# The hook should exit with non-zero status after issuing an
# appropriate message if it wants to stop the commit.  The hook is
# allowed to edit the commit message file.
#
# To enable this hook, rename this file to "applypatch-msg".

. git-sh-setup
commitmsg="$(git rev-parse --git-path hooks/commit-msg)"
test -x "$commitmsg" && exec "$commitmsg" ${1+"$@"}
:
````

## File: BackEnd/.git/hooks/commit-msg.sample
````
#!/bin/sh
#
# An example hook script to check the commit log message.
# Called by "git commit" with one argument, the name of the file
# that has the commit message.  The hook should exit with non-zero
# status after issuing an appropriate message if it wants to stop the
# commit.  The hook is allowed to edit the commit message file.
#
# To enable this hook, rename this file to "commit-msg".

# Uncomment the below to add a Signed-off-by line to the message.
# Doing this in a hook is a bad idea in general, but the prepare-commit-msg
# hook is more suited to it.
#
# SOB=$(git var GIT_AUTHOR_IDENT | sed -n 's/^\(.*>\).*$/Signed-off-by: \1/p')
# grep -qs "^$SOB" "$1" || echo "$SOB" >> "$1"

# This example catches duplicate Signed-off-by lines.

test "" = "$(grep '^Signed-off-by: ' "$1" |
	 sort | uniq -c | sed -e '/^[ 	]*1[ 	]/d')" || {
	echo >&2 Duplicate Signed-off-by lines.
	exit 1
}
````

## File: BackEnd/.git/hooks/fsmonitor-watchman.sample
````
#!/usr/bin/perl

use strict;
use warnings;
use IPC::Open2;

# An example hook script to integrate Watchman
# (https://facebook.github.io/watchman/) with git to speed up detecting
# new and modified files.
#
# The hook is passed a version (currently 2) and last update token
# formatted as a string and outputs to stdout a new update token and
# all files that have been modified since the update token. Paths must
# be relative to the root of the working tree and separated by a single NUL.
#
# To enable this hook, rename this file to "query-watchman" and set
# 'git config core.fsmonitor .git/hooks/query-watchman'
#
my ($version, $last_update_token) = @ARGV;

# Uncomment for debugging
# print STDERR "$0 $version $last_update_token\n";

# Check the hook interface version
if ($version ne 2) {
	die "Unsupported query-fsmonitor hook version '$version'.\n" .
	    "Falling back to scanning...\n";
}

my $git_work_tree = get_working_dir();

my $retry = 1;

my $json_pkg;
eval {
	require JSON::XS;
	$json_pkg = "JSON::XS";
	1;
} or do {
	require JSON::PP;
	$json_pkg = "JSON::PP";
};

launch_watchman();

sub launch_watchman {
	my $o = watchman_query();
	if (is_work_tree_watched($o)) {
		output_result($o->{clock}, @{$o->{files}});
	}
}

sub output_result {
	my ($clockid, @files) = @_;

	# Uncomment for debugging watchman output
	# open (my $fh, ">", ".git/watchman-output.out");
	# binmode $fh, ":utf8";
	# print $fh "$clockid\n@files\n";
	# close $fh;

	binmode STDOUT, ":utf8";
	print $clockid;
	print "\0";
	local $, = "\0";
	print @files;
}

sub watchman_clock {
	my $response = qx/watchman clock "$git_work_tree"/;
	die "Failed to get clock id on '$git_work_tree'.\n" .
		"Falling back to scanning...\n" if $? != 0;

	return $json_pkg->new->utf8->decode($response);
}

sub watchman_query {
	my $pid = open2(\*CHLD_OUT, \*CHLD_IN, 'watchman -j --no-pretty')
	or die "open2() failed: $!\n" .
	"Falling back to scanning...\n";

	# In the query expression below we're asking for names of files that
	# changed since $last_update_token but not from the .git folder.
	#
	# To accomplish this, we're using the "since" generator to use the
	# recency index to select candidate nodes and "fields" to limit the
	# output to file names only. Then we're using the "expression" term to
	# further constrain the results.
	my $last_update_line = "";
	if (substr($last_update_token, 0, 1) eq "c") {
		$last_update_token = "\"$last_update_token\"";
		$last_update_line = qq[\n"since": $last_update_token,];
	}
	my $query = <<"	END";
		["query", "$git_work_tree", {$last_update_line
			"fields": ["name"],
			"expression": ["not", ["dirname", ".git"]]
		}]
	END

	# Uncomment for debugging the watchman query
	# open (my $fh, ">", ".git/watchman-query.json");
	# print $fh $query;
	# close $fh;

	print CHLD_IN $query;
	close CHLD_IN;
	my $response = do {local $/; <CHLD_OUT>};

	# Uncomment for debugging the watch response
	# open ($fh, ">", ".git/watchman-response.json");
	# print $fh $response;
	# close $fh;

	die "Watchman: command returned no output.\n" .
	"Falling back to scanning...\n" if $response eq "";
	die "Watchman: command returned invalid output: $response\n" .
	"Falling back to scanning...\n" unless $response =~ /^\{/;

	return $json_pkg->new->utf8->decode($response);
}

sub is_work_tree_watched {
	my ($output) = @_;
	my $error = $output->{error};
	if ($retry > 0 and $error and $error =~ m/unable to resolve root .* directory (.*) is not watched/) {
		$retry--;
		my $response = qx/watchman watch "$git_work_tree"/;
		die "Failed to make watchman watch '$git_work_tree'.\n" .
		    "Falling back to scanning...\n" if $? != 0;
		$output = $json_pkg->new->utf8->decode($response);
		$error = $output->{error};
		die "Watchman: $error.\n" .
		"Falling back to scanning...\n" if $error;

		# Uncomment for debugging watchman output
		# open (my $fh, ">", ".git/watchman-output.out");
		# close $fh;

		# Watchman will always return all files on the first query so
		# return the fast "everything is dirty" flag to git and do the
		# Watchman query just to get it over with now so we won't pay
		# the cost in git to look up each individual file.
		my $o = watchman_clock();
		$error = $output->{error};

		die "Watchman: $error.\n" .
		"Falling back to scanning...\n" if $error;

		output_result($o->{clock}, ("/"));
		$last_update_token = $o->{clock};

		eval { launch_watchman() };
		return 0;
	}

	die "Watchman: $error.\n" .
	"Falling back to scanning...\n" if $error;

	return 1;
}

sub get_working_dir {
	my $working_dir;
	if ($^O =~ 'msys' || $^O =~ 'cygwin') {
		$working_dir = Win32::GetCwd();
		$working_dir =~ tr/\\/\//;
	} else {
		require Cwd;
		$working_dir = Cwd::cwd();
	}

	return $working_dir;
}
````

## File: BackEnd/.git/hooks/post-update.sample
````
#!/bin/sh
#
# An example hook script to prepare a packed repository for use over
# dumb transports.
#
# To enable this hook, rename this file to "post-update".

exec git update-server-info
````

## File: BackEnd/.git/hooks/pre-applypatch.sample
````
#!/bin/sh
#
# An example hook script to verify what is about to be committed
# by applypatch from an e-mail message.
#
# The hook should exit with non-zero status after issuing an
# appropriate message if it wants to stop the commit.
#
# To enable this hook, rename this file to "pre-applypatch".

. git-sh-setup
precommit="$(git rev-parse --git-path hooks/pre-commit)"
test -x "$precommit" && exec "$precommit" ${1+"$@"}
:
````

## File: BackEnd/.git/hooks/pre-commit.sample
````
#!/bin/sh
#
# An example hook script to verify what is about to be committed.
# Called by "git commit" with no arguments.  The hook should
# exit with non-zero status after issuing an appropriate message if
# it wants to stop the commit.
#
# To enable this hook, rename this file to "pre-commit".

if git rev-parse --verify HEAD >/dev/null 2>&1
then
	against=HEAD
else
	# Initial commit: diff against an empty tree object
	against=$(git hash-object -t tree /dev/null)
fi

# If you want to allow non-ASCII filenames set this variable to true.
allownonascii=$(git config --type=bool hooks.allownonascii)

# Redirect output to stderr.
exec 1>&2

# Cross platform projects tend to avoid non-ASCII filenames; prevent
# them from being added to the repository. We exploit the fact that the
# printable range starts at the space character and ends with tilde.
if [ "$allownonascii" != "true" ] &&
	# Note that the use of brackets around a tr range is ok here, (it's
	# even required, for portability to Solaris 10's /usr/bin/tr), since
	# the square bracket bytes happen to fall in the designated range.
	test $(git diff-index --cached --name-only --diff-filter=A -z $against |
	  LC_ALL=C tr -d '[ -~]\0' | wc -c) != 0
then
	cat <<\EOF
Error: Attempt to add a non-ASCII file name.

This can cause problems if you want to work with people on other platforms.

To be portable it is advisable to rename the file.

If you know what you are doing you can disable this check using:

  git config hooks.allownonascii true
EOF
	exit 1
fi

# If there are whitespace errors, print the offending file names and fail.
exec git diff-index --check --cached $against --
````

## File: BackEnd/.git/hooks/pre-merge-commit.sample
````
#!/bin/sh
#
# An example hook script to verify what is about to be committed.
# Called by "git merge" with no arguments.  The hook should
# exit with non-zero status after issuing an appropriate message to
# stderr if it wants to stop the merge commit.
#
# To enable this hook, rename this file to "pre-merge-commit".

. git-sh-setup
test -x "$GIT_DIR/hooks/pre-commit" &&
        exec "$GIT_DIR/hooks/pre-commit"
:
````

## File: BackEnd/.git/hooks/pre-push.sample
````
#!/bin/sh

# An example hook script to verify what is about to be pushed.  Called by "git
# push" after it has checked the remote status, but before anything has been
# pushed.  If this script exits with a non-zero status nothing will be pushed.
#
# This hook is called with the following parameters:
#
# $1 -- Name of the remote to which the push is being done
# $2 -- URL to which the push is being done
#
# If pushing without using a named remote those arguments will be equal.
#
# Information about the commits which are being pushed is supplied as lines to
# the standard input in the form:
#
#   <local ref> <local oid> <remote ref> <remote oid>
#
# This sample shows how to prevent push of commits where the log message starts
# with "WIP" (work in progress).

remote="$1"
url="$2"

zero=$(git hash-object --stdin </dev/null | tr '[0-9a-f]' '0')

while read local_ref local_oid remote_ref remote_oid
do
	if test "$local_oid" = "$zero"
	then
		# Handle delete
		:
	else
		if test "$remote_oid" = "$zero"
		then
			# New branch, examine all commits
			range="$local_oid"
		else
			# Update to existing branch, examine new commits
			range="$remote_oid..$local_oid"
		fi

		# Check for WIP commit
		commit=$(git rev-list -n 1 --grep '^WIP' "$range")
		if test -n "$commit"
		then
			echo >&2 "Found WIP commit in $local_ref, not pushing"
			exit 1
		fi
	fi
done

exit 0
````

## File: BackEnd/.git/hooks/pre-rebase.sample
````
#!/bin/sh
#
# Copyright (c) 2006, 2008 Junio C Hamano
#
# The "pre-rebase" hook is run just before "git rebase" starts doing
# its job, and can prevent the command from running by exiting with
# non-zero status.
#
# The hook is called with the following parameters:
#
# $1 -- the upstream the series was forked from.
# $2 -- the branch being rebased (or empty when rebasing the current branch).
#
# This sample shows how to prevent topic branches that are already
# merged to 'next' branch from getting rebased, because allowing it
# would result in rebasing already published history.

publish=next
basebranch="$1"
if test "$#" = 2
then
	topic="refs/heads/$2"
else
	topic=`git symbolic-ref HEAD` ||
	exit 0 ;# we do not interrupt rebasing detached HEAD
fi

case "$topic" in
refs/heads/??/*)
	;;
*)
	exit 0 ;# we do not interrupt others.
	;;
esac

# Now we are dealing with a topic branch being rebased
# on top of master.  Is it OK to rebase it?

# Does the topic really exist?
git show-ref -q "$topic" || {
	echo >&2 "No such branch $topic"
	exit 1
}

# Is topic fully merged to master?
not_in_master=`git rev-list --pretty=oneline ^master "$topic"`
if test -z "$not_in_master"
then
	echo >&2 "$topic is fully merged to master; better remove it."
	exit 1 ;# we could allow it, but there is no point.
fi

# Is topic ever merged to next?  If so you should not be rebasing it.
only_next_1=`git rev-list ^master "^$topic" ${publish} | sort`
only_next_2=`git rev-list ^master           ${publish} | sort`
if test "$only_next_1" = "$only_next_2"
then
	not_in_topic=`git rev-list "^$topic" master`
	if test -z "$not_in_topic"
	then
		echo >&2 "$topic is already up to date with master"
		exit 1 ;# we could allow it, but there is no point.
	else
		exit 0
	fi
else
	not_in_next=`git rev-list --pretty=oneline ^${publish} "$topic"`
	/usr/bin/perl -e '
		my $topic = $ARGV[0];
		my $msg = "* $topic has commits already merged to public branch:\n";
		my (%not_in_next) = map {
			/^([0-9a-f]+) /;
			($1 => 1);
		} split(/\n/, $ARGV[1]);
		for my $elem (map {
				/^([0-9a-f]+) (.*)$/;
				[$1 => $2];
			} split(/\n/, $ARGV[2])) {
			if (!exists $not_in_next{$elem->[0]}) {
				if ($msg) {
					print STDERR $msg;
					undef $msg;
				}
				print STDERR " $elem->[1]\n";
			}
		}
	' "$topic" "$not_in_next" "$not_in_master"
	exit 1
fi

<<\DOC_END

This sample hook safeguards topic branches that have been
published from being rewound.

The workflow assumed here is:

 * Once a topic branch forks from "master", "master" is never
   merged into it again (either directly or indirectly).

 * Once a topic branch is fully cooked and merged into "master",
   it is deleted.  If you need to build on top of it to correct
   earlier mistakes, a new topic branch is created by forking at
   the tip of the "master".  This is not strictly necessary, but
   it makes it easier to keep your history simple.

 * Whenever you need to test or publish your changes to topic
   branches, merge them into "next" branch.

The script, being an example, hardcodes the publish branch name
to be "next", but it is trivial to make it configurable via
$GIT_DIR/config mechanism.

With this workflow, you would want to know:

(1) ... if a topic branch has ever been merged to "next".  Young
    topic branches can have stupid mistakes you would rather
    clean up before publishing, and things that have not been
    merged into other branches can be easily rebased without
    affecting other people.  But once it is published, you would
    not want to rewind it.

(2) ... if a topic branch has been fully merged to "master".
    Then you can delete it.  More importantly, you should not
    build on top of it -- other people may already want to
    change things related to the topic as patches against your
    "master", so if you need further changes, it is better to
    fork the topic (perhaps with the same name) afresh from the
    tip of "master".

Let's look at this example:

		   o---o---o---o---o---o---o---o---o---o "next"
		  /       /           /           /
		 /   a---a---b A     /           /
		/   /               /           /
	       /   /   c---c---c---c B         /
	      /   /   /             \         /
	     /   /   /   b---b C     \       /
	    /   /   /   /             \     /
    ---o---o---o---o---o---o---o---o---o---o---o "master"


A, B and C are topic branches.

 * A has one fix since it was merged up to "next".

 * B has finished.  It has been fully merged up to "master" and "next",
   and is ready to be deleted.

 * C has not merged to "next" at all.

We would want to allow C to be rebased, refuse A, and encourage
B to be deleted.

To compute (1):

	git rev-list ^master ^topic next
	git rev-list ^master        next

	if these match, topic has not merged in next at all.

To compute (2):

	git rev-list master..topic

	if this is empty, it is fully merged to "master".

DOC_END
````

## File: BackEnd/.git/hooks/pre-receive.sample
````
#!/bin/sh
#
# An example hook script to make use of push options.
# The example simply echoes all push options that start with 'echoback='
# and rejects all pushes when the "reject" push option is used.
#
# To enable this hook, rename this file to "pre-receive".

if test -n "$GIT_PUSH_OPTION_COUNT"
then
	i=0
	while test "$i" -lt "$GIT_PUSH_OPTION_COUNT"
	do
		eval "value=\$GIT_PUSH_OPTION_$i"
		case "$value" in
		echoback=*)
			echo "echo from the pre-receive-hook: ${value#*=}" >&2
			;;
		reject)
			exit 1
		esac
		i=$((i + 1))
	done
fi
````

## File: BackEnd/.git/hooks/prepare-commit-msg.sample
````
#!/bin/sh
#
# An example hook script to prepare the commit log message.
# Called by "git commit" with the name of the file that has the
# commit message, followed by the description of the commit
# message's source.  The hook's purpose is to edit the commit
# message file.  If the hook fails with a non-zero status,
# the commit is aborted.
#
# To enable this hook, rename this file to "prepare-commit-msg".

# This hook includes three examples. The first one removes the
# "# Please enter the commit message..." help message.
#
# The second includes the output of "git diff --name-status -r"
# into the message, just before the "git status" output.  It is
# commented because it doesn't cope with --amend or with squashed
# commits.
#
# The third example adds a Signed-off-by line to the message, that can
# still be edited.  This is rarely a good idea.

COMMIT_MSG_FILE=$1
COMMIT_SOURCE=$2
SHA1=$3

/usr/bin/perl -i.bak -ne 'print unless(m/^. Please enter the commit message/..m/^#$/)' "$COMMIT_MSG_FILE"

# case "$COMMIT_SOURCE,$SHA1" in
#  ,|template,)
#    /usr/bin/perl -i.bak -pe '
#       print "\n" . `git diff --cached --name-status -r`
# 	 if /^#/ && $first++ == 0' "$COMMIT_MSG_FILE" ;;
#  *) ;;
# esac

# SOB=$(git var GIT_COMMITTER_IDENT | sed -n 's/^\(.*>\).*$/Signed-off-by: \1/p')
# git interpret-trailers --in-place --trailer "$SOB" "$COMMIT_MSG_FILE"
# if test -z "$COMMIT_SOURCE"
# then
#   /usr/bin/perl -i.bak -pe 'print "\n" if !$first_line++' "$COMMIT_MSG_FILE"
# fi
````

## File: BackEnd/.git/hooks/push-to-checkout.sample
````
#!/bin/sh

# An example hook script to update a checked-out tree on a git push.
#
# This hook is invoked by git-receive-pack(1) when it reacts to git
# push and updates reference(s) in its repository, and when the push
# tries to update the branch that is currently checked out and the
# receive.denyCurrentBranch configuration variable is set to
# updateInstead.
#
# By default, such a push is refused if the working tree and the index
# of the remote repository has any difference from the currently
# checked out commit; when both the working tree and the index match
# the current commit, they are updated to match the newly pushed tip
# of the branch. This hook is to be used to override the default
# behaviour; however the code below reimplements the default behaviour
# as a starting point for convenient modification.
#
# The hook receives the commit with which the tip of the current
# branch is going to be updated:
commit=$1

# It can exit with a non-zero status to refuse the push (when it does
# so, it must not modify the index or the working tree).
die () {
	echo >&2 "$*"
	exit 1
}

# Or it can make any necessary changes to the working tree and to the
# index to bring them to the desired state when the tip of the current
# branch is updated to the new commit, and exit with a zero status.
#
# For example, the hook can simply run git read-tree -u -m HEAD "$1"
# in order to emulate git fetch that is run in the reverse direction
# with git push, as the two-tree form of git read-tree -u -m is
# essentially the same as git switch or git checkout that switches
# branches while keeping the local changes in the working tree that do
# not interfere with the difference between the branches.

# The below is a more-or-less exact translation to shell of the C code
# for the default behaviour for git's push-to-checkout hook defined in
# the push_to_deploy() function in builtin/receive-pack.c.
#
# Note that the hook will be executed from the repository directory,
# not from the working tree, so if you want to perform operations on
# the working tree, you will have to adapt your code accordingly, e.g.
# by adding "cd .." or using relative paths.

if ! git update-index -q --ignore-submodules --refresh
then
	die "Up-to-date check failed"
fi

if ! git diff-files --quiet --ignore-submodules --
then
	die "Working directory has unstaged changes"
fi

# This is a rough translation of:
#
#   head_has_history() ? "HEAD" : EMPTY_TREE_SHA1_HEX
if git cat-file -e HEAD 2>/dev/null
then
	head=HEAD
else
	head=$(git hash-object -t tree --stdin </dev/null)
fi

if ! git diff-index --quiet --cached --ignore-submodules $head --
then
	die "Working directory has staged changes"
fi

if ! git read-tree -u -m "$commit"
then
	die "Could not update working tree to new HEAD"
fi
````

## File: BackEnd/.git/hooks/sendemail-validate.sample
````
#!/bin/sh

# An example hook script to validate a patch (and/or patch series) before
# sending it via email.
#
# The hook should exit with non-zero status after issuing an appropriate
# message if it wants to prevent the email(s) from being sent.
#
# To enable this hook, rename this file to "sendemail-validate".
#
# By default, it will only check that the patch(es) can be applied on top of
# the default upstream branch without conflicts in a secondary worktree. After
# validation (successful or not) of the last patch of a series, the worktree
# will be deleted.
#
# The following config variables can be set to change the default remote and
# remote ref that are used to apply the patches against:
#
#   sendemail.validateRemote (default: origin)
#   sendemail.validateRemoteRef (default: HEAD)
#
# Replace the TODO placeholders with appropriate checks according to your
# needs.

validate_cover_letter () {
	file="$1"
	# TODO: Replace with appropriate checks (e.g. spell checking).
	true
}

validate_patch () {
	file="$1"
	# Ensure that the patch applies without conflicts.
	git am -3 "$file" || return
	# TODO: Replace with appropriate checks for this patch
	# (e.g. checkpatch.pl).
	true
}

validate_series () {
	# TODO: Replace with appropriate checks for the whole series
	# (e.g. quick build, coding style checks, etc.).
	true
}

# main -------------------------------------------------------------------------

if test "$GIT_SENDEMAIL_FILE_COUNTER" = 1
then
	remote=$(git config --default origin --get sendemail.validateRemote) &&
	ref=$(git config --default HEAD --get sendemail.validateRemoteRef) &&
	worktree=$(mktemp --tmpdir -d sendemail-validate.XXXXXXX) &&
	git worktree add -fd --checkout "$worktree" "refs/remotes/$remote/$ref" &&
	git config --replace-all sendemail.validateWorktree "$worktree"
else
	worktree=$(git config --get sendemail.validateWorktree)
fi || {
	echo "sendemail-validate: error: failed to prepare worktree" >&2
	exit 1
}

unset GIT_DIR GIT_WORK_TREE
cd "$worktree" &&

if grep -q "^diff --git " "$1"
then
	validate_patch "$1"
else
	validate_cover_letter "$1"
fi &&

if test "$GIT_SENDEMAIL_FILE_COUNTER" = "$GIT_SENDEMAIL_FILE_TOTAL"
then
	git config --unset-all sendemail.validateWorktree &&
	trap 'git worktree remove -ff "$worktree"' EXIT &&
	validate_series
fi
````

## File: BackEnd/.git/hooks/update.sample
````
#!/bin/sh
#
# An example hook script to block unannotated tags from entering.
# Called by "git receive-pack" with arguments: refname sha1-old sha1-new
#
# To enable this hook, rename this file to "update".
#
# Config
# ------
# hooks.allowunannotated
#   This boolean sets whether unannotated tags will be allowed into the
#   repository.  By default they won't be.
# hooks.allowdeletetag
#   This boolean sets whether deleting tags will be allowed in the
#   repository.  By default they won't be.
# hooks.allowmodifytag
#   This boolean sets whether a tag may be modified after creation. By default
#   it won't be.
# hooks.allowdeletebranch
#   This boolean sets whether deleting branches will be allowed in the
#   repository.  By default they won't be.
# hooks.denycreatebranch
#   This boolean sets whether remotely creating branches will be denied
#   in the repository.  By default this is allowed.
#

# --- Command line
refname="$1"
oldrev="$2"
newrev="$3"

# --- Safety check
if [ -z "$GIT_DIR" ]; then
	echo "Don't run this script from the command line." >&2
	echo " (if you want, you could supply GIT_DIR then run" >&2
	echo "  $0 <ref> <oldrev> <newrev>)" >&2
	exit 1
fi

if [ -z "$refname" -o -z "$oldrev" -o -z "$newrev" ]; then
	echo "usage: $0 <ref> <oldrev> <newrev>" >&2
	exit 1
fi

# --- Config
allowunannotated=$(git config --type=bool hooks.allowunannotated)
allowdeletebranch=$(git config --type=bool hooks.allowdeletebranch)
denycreatebranch=$(git config --type=bool hooks.denycreatebranch)
allowdeletetag=$(git config --type=bool hooks.allowdeletetag)
allowmodifytag=$(git config --type=bool hooks.allowmodifytag)

# check for no description
projectdesc=$(sed -e '1q' "$GIT_DIR/description")
case "$projectdesc" in
"Unnamed repository"* | "")
	echo "*** Project description file hasn't been set" >&2
	exit 1
	;;
esac

# --- Check types
# if $newrev is 0000...0000, it's a commit to delete a ref.
zero=$(git hash-object --stdin </dev/null | tr '[0-9a-f]' '0')
if [ "$newrev" = "$zero" ]; then
	newrev_type=delete
else
	newrev_type=$(git cat-file -t $newrev)
fi

case "$refname","$newrev_type" in
	refs/tags/*,commit)
		# un-annotated tag
		short_refname=${refname##refs/tags/}
		if [ "$allowunannotated" != "true" ]; then
			echo "*** The un-annotated tag, $short_refname, is not allowed in this repository" >&2
			echo "*** Use 'git tag [ -a | -s ]' for tags you want to propagate." >&2
			exit 1
		fi
		;;
	refs/tags/*,delete)
		# delete tag
		if [ "$allowdeletetag" != "true" ]; then
			echo "*** Deleting a tag is not allowed in this repository" >&2
			exit 1
		fi
		;;
	refs/tags/*,tag)
		# annotated tag
		if [ "$allowmodifytag" != "true" ] && git rev-parse $refname > /dev/null 2>&1
		then
			echo "*** Tag '$refname' already exists." >&2
			echo "*** Modifying a tag is not allowed in this repository." >&2
			exit 1
		fi
		;;
	refs/heads/*,commit)
		# branch
		if [ "$oldrev" = "$zero" -a "$denycreatebranch" = "true" ]; then
			echo "*** Creating a branch is not allowed in this repository" >&2
			exit 1
		fi
		;;
	refs/heads/*,delete)
		# delete branch
		if [ "$allowdeletebranch" != "true" ]; then
			echo "*** Deleting a branch is not allowed in this repository" >&2
			exit 1
		fi
		;;
	refs/remotes/*,commit)
		# tracking branch
		;;
	refs/remotes/*,delete)
		# delete tracking branch
		if [ "$allowdeletebranch" != "true" ]; then
			echo "*** Deleting a tracking branch is not allowed in this repository" >&2
			exit 1
		fi
		;;
	*)
		# Anything else (is there anything else?)
		echo "*** Update hook: unknown type of update to ref $refname of type $newrev_type" >&2
		exit 1
		;;
esac

# --- Finished
exit 0
````

## File: BackEnd/.git/info/exclude
````
# git ls-files --others --exclude-from=.git/info/exclude
# Lines that start with '#' are comments.
# For a project mostly in C, the following would be a good set of
# exclude patterns (uncomment them if you want to use them):
# *.[oa]
# *~
````

## File: BackEnd/.git/logs/HEAD
````
0000000000000000000000000000000000000000 6e7d2815f0e46bf3b7a82dffdd9929d48f8bd540 Chalithya <schalithya@gmail.com> 1750788268 -0400	clone: from https://github.com/rajatsachdeva31/ImmiGrowAI-BackEnd.git
````

## File: BackEnd/.git/logs/refs/heads/main
````
0000000000000000000000000000000000000000 6e7d2815f0e46bf3b7a82dffdd9929d48f8bd540 Chalithya <schalithya@gmail.com> 1750788268 -0400	clone: from https://github.com/rajatsachdeva31/ImmiGrowAI-BackEnd.git
````

## File: BackEnd/.git/logs/refs/remotes/origin/HEAD
````
0000000000000000000000000000000000000000 6e7d2815f0e46bf3b7a82dffdd9929d48f8bd540 Chalithya <schalithya@gmail.com> 1750788268 -0400	clone: from https://github.com/rajatsachdeva31/ImmiGrowAI-BackEnd.git
````

## File: BackEnd/.git/packed-refs
````
# pack-refs with: peeled fully-peeled sorted 
6e7d2815f0e46bf3b7a82dffdd9929d48f8bd540 refs/remotes/origin/main
````

## File: BackEnd/.git/refs/heads/main
````
6e7d2815f0e46bf3b7a82dffdd9929d48f8bd540
````

## File: BackEnd/.git/refs/remotes/origin/HEAD
````
ref: refs/remotes/origin/main
````

## File: BackEnd/.gitignore
````
# Node.js dependencies
node_modules/

# Logs
logs/
*.log
npm-debug.log*

# Environment variables
.env

# Build outputs
dist/
build/

# System files
.DS_Store
Thumbs.db

# IDE settings
.vscode/
.idea/

# Firebase Admin Credentials
serviceAccountKey.json

#test files
tes.html
testPasswordencryption.html
testforgotpassword.html
testresend.html
downloadtest.html
check.html
carlistingtest.html
downloadtest.html
houselistingtest.html
testframe.html
````

## File: BackEnd/index.js
````javascript
// server.js
const express = require("express");
const cors = require("cors");
const cookieParser = require("cookie-parser"); // Import cookie-parser
require("dotenv").config(); // Load environment variables
const admin = require("./middleware/firebaseAdminMiddleware");
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();

const userRoutes = require('./routes/authRoutes'); 
const onboardingRoutes = require('./routes/onboardingRoutes'); 
const dashboardRoutes = require('./routes/dashboardRoutes'); 
const adminVerificationRoutes = require('./routes/admin/verifyUserRoute'); 
const adminUserRoutes = require('./routes/admin/userDetailsRoute'); 
const adminStatsRoutes = require('./routes/admin/adminStatsRoute'); 
const houseListingRoutes = require("./routes/houseListingRoutes");
const carListingRoutes = require("./routes/carListingRoutes");
const availabilityRoutes = require("./routes/availabilityRoutes");
const appointmentRoutes = require("./routes/appointment");
const calAuthRoutes = require("./routes/calendarAuthRoutes");
const consultantRoutes = require("./routes/consultantRoutes");

const app = express();
app.use(express.urlencoded({ extended: true }));

const corsOptions = {
  origin: ["http://localhost:3000", "http://127.0.0.1:3000","http://localhost:5500", "http://127.0.0.1:5500","http://localhost:5501", "http://127.0.0.1:5501"], // Add both origins
  credentials: true, // Allow cookies and credentials
  methods: "GET,HEAD,PUT,PATCH,POST,DELETE,OPTIONS",
  allowedHeaders: "Content-Type,Authorization",
};


// Middleware
app.use( cors({
  origin: ["http://localhost:3000", "http://127.0.0.1:3000","http://localhost:5500", "http://127.0.0.1:5500","http://localhost:5501", "http://127.0.0.1:5501"], // Add both origins
  credentials: true, // Allow cookies and credentials
  methods: "GET,HEAD,PUT,PATCH,POST,DELETE,OPTIONS",
  allowedHeaders: "Content-Type,Authorization",
}));

app.options("*", cors(corsOptions));
app.use(express.json());
app.use(cookieParser()); // Add cookie parser

app.get("/auth/token", async (req, res) => {
  const token = req.cookies.token;
 const decodedToken = await admin.auth().verifyIdToken(token);
 const user = await prisma.user.findUnique({
  where: {
    email: decodedToken.email
  },
  include: {
    role: true
  }
});

let roleName = user?.role?.name;
const verification = user?.userVerified;

if (!roleName) {
    roleName = "Onboarding";
}
else if (verification === false) {
  roleName = "NotVerified";
}

  if (!token) return res.status(401).json({ message: "Unauthorized" });

  res.json({ token, roleName });
});


// Routes
app.use("/api/users", userRoutes);
app.use("/api/onboarding", onboardingRoutes);
app.use("/api/admin/verify", adminVerificationRoutes);
app.use("/api/admin/user-list", adminUserRoutes);
app.use("/api/admin/dashboard", adminStatsRoutes);
app.use("/api/protected/", dashboardRoutes);
app.use("/api/protected/house-listing", houseListingRoutes);
app.use("/api/protected/car-listing", carListingRoutes);
app.use("/api/protected/consultants", consultantRoutes);
app.use("/api/protected/availability", availabilityRoutes);
app.use("/api/protected/appointment", appointmentRoutes);
app.use("/api/protected/oauth", calAuthRoutes);
// Start server
const PORT = process.env.PORT || 5500;
app.listen(PORT, () => {
  console.log(`Server running on port ${PORT}`);
});
````

## File: BackEnd/middleware/authMiddleware.js
````javascript
const admin = require('../middleware/firebaseAdminMiddleware'); 

// Middleware to verify Firebase token
const verifyToken = async (req, res, next) => {
  const authHeader = req.headers.authorization;

  if (!authHeader || !authHeader.startsWith("Bearer ")) {
    return res.status(401).json({ error: "Unauthorized. Token is missing or invalid." });
  }

  const token = authHeader.split(" ")[1];

  try {
    // Verify the token using Firebase Admin SDK
    const decodedToken = await admin.auth().verifyIdToken(token);
    req.user = decodedToken; // Attach decoded user data to the request
    next(); // Pass to the next middleware/route handler
  } catch (error) {
    return res.status(403).json({ error: "Forbidden. Invalid or expired token." });
  }
};

module.exports = verifyToken;
````

## File: BackEnd/middleware/decryptionMiddleware.js
````javascript
const crypto = require("crypto");
require("dotenv").config();

const SECRET_KEY = Buffer.from(process.env.AES_SECRET_KEY, "utf8");

const decryptPasswordMiddleware = (req, res, next) => {
  try {
    const { password, iv } = req.body;

    if (!password || !iv) {
      return res.status(400).json({ error: "Password and IV are required" });
    }

    // Decrypt the password
    const decipher = crypto.createDecipheriv("aes-256-cbc", SECRET_KEY, Buffer.from(iv, "hex"));
    let decryptedPassword = decipher.update(password, "base64", "utf8");
    decryptedPassword += decipher.final("utf8");


    // Replace the encrypted password in the request body with the decrypted one
    req.body.password = decryptedPassword;

    next(); // Pass control to the next middleware or route handler
  } catch (error) {
    res.status(400).json({ error: "Failed to decrypt password", details: error.message });
  }
};

module.exports = decryptPasswordMiddleware;
````

## File: BackEnd/middleware/firebaseAdminMiddleware.js
````javascript
const admin = require("firebase-admin");

if (!admin.apps.length) {
  // Initialize Firebase Admin SDK
const serviceAccount = require("../serviceAccountKey.json");
admin.initializeApp({
  credential: admin.credential.cert(serviceAccount),
});

}

module.exports = admin;
````

## File: BackEnd/middleware/oauthTokenMiddleware.js
````javascript
const { google } = require('googleapis');
require('dotenv').config();

const oauth2Client = new google.auth.OAuth2(
    process.env.GOOGLE_CLIENT_ID,
    process.env.GOOGLE_CLIENT_SECRET,
    process.env.GOOGLE_REDIRECT_URI,
);

async function getAccessToken(refreshToken) {
    oauth2Client.setCredentials({ refresh_token: refreshToken });
    const { credentials } = await oauth2Client.refreshAccessToken();
    return credentials.access_token;
}

module.exports = { getAccessToken };
````

## File: BackEnd/middleware/roleBasedDataMiddleware.js
````javascript
const { PrismaClient } = require("@prisma/client");
const prisma = new PrismaClient();

const roleBasedData = async (req, res, next) => {
  try {

    // find role based on rolename
    const role = await prisma.role.findUnique({
      where: {
        name: req.body.rolename,
      },
    });

    if (!role) {
      return res.status(404).json({ error: "Role not found" });
    }

    req.body.roleId = role.id;

    // Additional checks based on the role

    if (role.name === "Realtor") {
      req.body.realtorData = {
        businessName: req.body.businessName,
        businessAddress: req.body.businessAddress || null,
        realEstateLicenseNumber: req.body.realEstateLicenseNumber,
        yearsOfExperience: req.body.experienceYears,
        affiliatedAssociations: req.body.affiliatedAssociations || null,
        areasCovered: req.body.areasCovered,
        specialties: req.body.specialties,
        portfolioWebsite: req.body.portfolioLink || null,
        businessRegistration: req.body.registrationNumber,
        workType:
          req.body.workType == "Brokerage" ? "BROKERAGE" : "INDEPENDENT",
        brokerageName: null,
        teamMembers: parseInt(req.body.teamMembers, 10),
        officeLocationAvailable:
          JSON.parse(req.body.officeLocationAvailable) || false,
        virtualPropertyTour: JSON.parse(req.body.virtualPropertyTour) || false,
      };

      if (req.body.realtorData.workType == "BROKERAGE") {
        req.body.realtorData.brokerageName = req.body.brokerageName;
      }
    } else if (role.name === "Car Dealership") {
      req.body.carDealershipData = {
        showroomLocations: req.body.showroomLocations,
        testDrivePolicy: req.body.testDrivePolicy,
        financingOptions: req.body.financingOptions,
        tradeInAvailable: JSON.parse(req.body.tradeInOptions) || false,
        serviceWarrantyInfo: req.body.serviceWarrantyInfo,
        businessRegistration: req.body.businessRegistration,
        businessName: req.body.businessName,
        yearsInBusiness: req.body.yearsInBusiness,
        dealershipLicenseNumber: req.body.dealershipLicenseNumber,
        carBrandsSold: req.body.carBrandsSold,
        newOrUsedCars: req.body.newOrUsedCars,
      };
    } else if (role.name === "Immigration Consultant") {
      req.body.immigrationConsultantData = {
        countriesServed: req.body.countriesServed,
        consultationFee: Number(req.body.consultationFee) || null,
        businessRegistration: req.body.businessRegistration,
        partneredLegalFirms: req.body.legalFirms || null,
        businessName: req.body.businessName,
        businessAddress: req.body.businessAddress,
        yearsOfExperience: req.body.yearsOfExperience,
        licenseNumber: req.body.licenseNumber,
        servicesOffered: req.body.servicesOffered,
        websiteOrSocialMedia: req.body.websiteLink || null,
        languagesSpoken: req.body.languagesSpoken,
      };
    }

    next();
  } catch (error) {
    console.error("Error in roleBasedData middleware:", error.message);
    res.status(500).json({ error: "Internal server error" });
  }
};

module.exports = roleBasedData;
````

## File: BackEnd/middleware/uploadFileMiddleware.js
````javascript
const multer = require('multer');

const storage = multer.memoryStorage();

const fileFilter = (req, file, cb) => {
    if (req.body.rolename === 'Immigrant') {
        if (file.fieldname === 'govId') {
            return cb(null, true);
        }
        return cb(new Error('Immigrants can only upload Government ID.'));
    }

    // Other roles can upload all three
    return cb(null, true);
};

const upload = multer({ storage, fileFilter });

const uploadFileMiddleware = upload.fields([
    { name: 'govId', maxCount: 1 },
    { name: 'businessDoc', maxCount: 1 },
    { name: 'licenseCert', maxCount: 1 }
]);

module.exports = uploadFileMiddleware;
````

## File: BackEnd/middleware/uploadMiddleware.js
````javascript
const multer = require('multer');

// Configure Multer for in-memory storage
const storage = multer.memoryStorage();
const upload = multer({ storage: storage });

// Middleware for handling multiple file uploads
const uploadimage = upload.fields([
  { name: 'imageOne', maxCount: 1 },
  { name: 'imageTwo', maxCount: 1 },
  { name: 'imageThree', maxCount: 1 }
]);

module.exports = uploadimage;
````

## File: BackEnd/package.json
````json
{
  "name": "immigratexai-backend",
  "version": "1.0.0",
  "description": "This is backend for ImmigrateX.ai web app",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "dev": "nodemon ./index.js",
    "prisma:seed": "node prisma/seed.js"
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "@prisma/client": "^6.5.0",
    "axios": "^1.7.9",
    "body-parser": "^1.20.3",
    "cookie-parser": "^1.4.7",
    "cors": "^2.8.5",
    "debug": "^4.4.0",
    "dotenv": "^16.4.7",
    "express": "^4.21.2",
    "express-session": "^1.18.1",
    "firebase-admin": "^13.0.2",
    "googleapis": "^146.0.0",
    "iconv-lite": "^0.6.3",
    "jsonwebtoken": "^9.0.2",
    "mailgen": "^2.0.29",
    "mailtrap": "^3.4.0",
    "multer": "^1.4.5-lts.1",
    "nodemailer": "^6.10.0",
    "nodemon": "^3.1.9",
    "pg": "^8.13.1",
    "readline-sync": "^1.4.10"
  },
  "devDependencies": {
    "prisma": "^6.5.0"
  }
}
````

## File: BackEnd/prisma/migrations/20250201195516_init/migration.sql
````sql
-- CreateTable
CREATE TABLE "User" (
    "id" TEXT NOT NULL,
    "email" TEXT NOT NULL,
    "firebaseUid" TEXT NOT NULL,
    "roleId" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "User_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "Role" (
    "id" TEXT NOT NULL,
    "name" TEXT NOT NULL,

    CONSTRAINT "Role_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "HouseListing" (
    "id" TEXT NOT NULL,
    "title" TEXT NOT NULL,
    "description" TEXT,
    "price" DECIMAL(65,30) NOT NULL,
    "location" TEXT NOT NULL,
    "landlordId" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "HouseListing_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "CarListing" (
    "id" TEXT NOT NULL,
    "model" TEXT NOT NULL,
    "make" TEXT NOT NULL,
    "price" DECIMAL(65,30) NOT NULL,
    "dealershipId" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "CarListing_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "HouseBooking" (
    "id" TEXT NOT NULL,
    "userId" TEXT NOT NULL,
    "listingId" TEXT NOT NULL,
    "startDate" TIMESTAMP(3) NOT NULL,
    "endDate" TIMESTAMP(3) NOT NULL,
    "status" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "HouseBooking_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "CarBooking" (
    "id" TEXT NOT NULL,
    "userId" TEXT NOT NULL,
    "listingId" TEXT NOT NULL,
    "startDate" TIMESTAMP(3) NOT NULL,
    "endDate" TIMESTAMP(3) NOT NULL,
    "status" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "CarBooking_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "UserDocument" (
    "id" TEXT NOT NULL,
    "userId" TEXT NOT NULL,
    "documentType" TEXT NOT NULL,
    "fileData" BYTEA NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "UserDocument_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "PropertyDocument" (
    "id" TEXT NOT NULL,
    "listingId" TEXT NOT NULL,
    "documentType" TEXT NOT NULL,
    "fileData" BYTEA NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "PropertyDocument_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "CarDocument" (
    "id" TEXT NOT NULL,
    "listingId" TEXT NOT NULL,
    "documentType" TEXT NOT NULL,
    "fileData" BYTEA NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "CarDocument_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "Checklist" (
    "id" TEXT NOT NULL,
    "name" TEXT NOT NULL,
    "type" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "Checklist_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "UserChecklistItem" (
    "id" TEXT NOT NULL,
    "userId" TEXT NOT NULL,
    "checklistId" TEXT NOT NULL,
    "status" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "UserChecklistItem_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "Consultation" (
    "id" TEXT NOT NULL,
    "consultantId" TEXT NOT NULL,
    "availableAt" TIMESTAMP(3) NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "Consultation_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "Appointment" (
    "id" TEXT NOT NULL,
    "userId" TEXT NOT NULL,
    "consultationId" TEXT NOT NULL,
    "status" TEXT NOT NULL,
    "bookedAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "Appointment_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "Payment" (
    "id" TEXT NOT NULL,
    "userId" TEXT NOT NULL,
    "amount" DECIMAL(65,30) NOT NULL,
    "transactionType" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "Payment_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "HouseImage" (
    "id" TEXT NOT NULL,
    "listingId" TEXT NOT NULL,
    "imageData" BYTEA NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "HouseImage_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "CarImage" (
    "id" TEXT NOT NULL,
    "listingId" TEXT NOT NULL,
    "imageData" BYTEA NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "CarImage_pkey" PRIMARY KEY ("id")
);

-- CreateIndex
CREATE UNIQUE INDEX "User_email_key" ON "User"("email");

-- CreateIndex
CREATE UNIQUE INDEX "User_firebaseUid_key" ON "User"("firebaseUid");

-- CreateIndex
CREATE UNIQUE INDEX "Role_name_key" ON "Role"("name");

-- AddForeignKey
ALTER TABLE "User" ADD CONSTRAINT "User_roleId_fkey" FOREIGN KEY ("roleId") REFERENCES "Role"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "HouseListing" ADD CONSTRAINT "HouseListing_landlordId_fkey" FOREIGN KEY ("landlordId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarListing" ADD CONSTRAINT "CarListing_dealershipId_fkey" FOREIGN KEY ("dealershipId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "HouseBooking" ADD CONSTRAINT "HouseBooking_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "HouseBooking" ADD CONSTRAINT "HouseBooking_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "HouseListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarBooking" ADD CONSTRAINT "CarBooking_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarBooking" ADD CONSTRAINT "CarBooking_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "CarListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "UserDocument" ADD CONSTRAINT "UserDocument_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "PropertyDocument" ADD CONSTRAINT "PropertyDocument_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "HouseListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarDocument" ADD CONSTRAINT "CarDocument_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "CarListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "UserChecklistItem" ADD CONSTRAINT "UserChecklistItem_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "UserChecklistItem" ADD CONSTRAINT "UserChecklistItem_checklistId_fkey" FOREIGN KEY ("checklistId") REFERENCES "Checklist"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "Consultation" ADD CONSTRAINT "Consultation_consultantId_fkey" FOREIGN KEY ("consultantId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "Appointment" ADD CONSTRAINT "Appointment_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "Appointment" ADD CONSTRAINT "Appointment_consultationId_fkey" FOREIGN KEY ("consultationId") REFERENCES "Consultation"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "Payment" ADD CONSTRAINT "Payment_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "HouseImage" ADD CONSTRAINT "HouseImage_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "HouseListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarImage" ADD CONSTRAINT "CarImage_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "CarListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;
````

## File: BackEnd/prisma/migrations/20250201200911_change_ids_to_int/migration.sql
````sql
/*
  Warnings:

  - The primary key for the `Appointment` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `Appointment` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `CarBooking` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `CarBooking` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `CarDocument` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `CarDocument` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `CarImage` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `CarImage` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `CarListing` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `CarListing` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `Checklist` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `Checklist` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `Consultation` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `Consultation` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `HouseBooking` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `HouseBooking` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `HouseImage` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `HouseImage` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `HouseListing` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `HouseListing` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `Payment` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `Payment` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `PropertyDocument` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `PropertyDocument` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `Role` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `Role` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `User` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `User` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `UserChecklistItem` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `UserChecklistItem` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - The primary key for the `UserDocument` table will be changed. If it partially fails, the table could be left without primary key constraint.
  - The `id` column on the `UserDocument` table would be dropped and recreated. This will lead to data loss if there is data in the column.
  - Changed the type of `userId` on the `Appointment` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `consultationId` on the `Appointment` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `userId` on the `CarBooking` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `listingId` on the `CarBooking` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `listingId` on the `CarDocument` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `listingId` on the `CarImage` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `dealershipId` on the `CarListing` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `consultantId` on the `Consultation` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `userId` on the `HouseBooking` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `listingId` on the `HouseBooking` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `listingId` on the `HouseImage` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `landlordId` on the `HouseListing` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `userId` on the `Payment` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `listingId` on the `PropertyDocument` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `roleId` on the `User` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `userId` on the `UserChecklistItem` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `checklistId` on the `UserChecklistItem` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `userId` on the `UserDocument` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.

*/
-- DropForeignKey
ALTER TABLE "Appointment" DROP CONSTRAINT "Appointment_consultationId_fkey";

-- DropForeignKey
ALTER TABLE "Appointment" DROP CONSTRAINT "Appointment_userId_fkey";

-- DropForeignKey
ALTER TABLE "CarBooking" DROP CONSTRAINT "CarBooking_listingId_fkey";

-- DropForeignKey
ALTER TABLE "CarBooking" DROP CONSTRAINT "CarBooking_userId_fkey";

-- DropForeignKey
ALTER TABLE "CarDocument" DROP CONSTRAINT "CarDocument_listingId_fkey";

-- DropForeignKey
ALTER TABLE "CarImage" DROP CONSTRAINT "CarImage_listingId_fkey";

-- DropForeignKey
ALTER TABLE "CarListing" DROP CONSTRAINT "CarListing_dealershipId_fkey";

-- DropForeignKey
ALTER TABLE "Consultation" DROP CONSTRAINT "Consultation_consultantId_fkey";

-- DropForeignKey
ALTER TABLE "HouseBooking" DROP CONSTRAINT "HouseBooking_listingId_fkey";

-- DropForeignKey
ALTER TABLE "HouseBooking" DROP CONSTRAINT "HouseBooking_userId_fkey";

-- DropForeignKey
ALTER TABLE "HouseImage" DROP CONSTRAINT "HouseImage_listingId_fkey";

-- DropForeignKey
ALTER TABLE "HouseListing" DROP CONSTRAINT "HouseListing_landlordId_fkey";

-- DropForeignKey
ALTER TABLE "Payment" DROP CONSTRAINT "Payment_userId_fkey";

-- DropForeignKey
ALTER TABLE "PropertyDocument" DROP CONSTRAINT "PropertyDocument_listingId_fkey";

-- DropForeignKey
ALTER TABLE "User" DROP CONSTRAINT "User_roleId_fkey";

-- DropForeignKey
ALTER TABLE "UserChecklistItem" DROP CONSTRAINT "UserChecklistItem_checklistId_fkey";

-- DropForeignKey
ALTER TABLE "UserChecklistItem" DROP CONSTRAINT "UserChecklistItem_userId_fkey";

-- DropForeignKey
ALTER TABLE "UserDocument" DROP CONSTRAINT "UserDocument_userId_fkey";

-- AlterTable
ALTER TABLE "Appointment" DROP CONSTRAINT "Appointment_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "userId",
ADD COLUMN     "userId" INTEGER NOT NULL,
DROP COLUMN "consultationId",
ADD COLUMN     "consultationId" INTEGER NOT NULL,
ADD CONSTRAINT "Appointment_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "CarBooking" DROP CONSTRAINT "CarBooking_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "userId",
ADD COLUMN     "userId" INTEGER NOT NULL,
DROP COLUMN "listingId",
ADD COLUMN     "listingId" INTEGER NOT NULL,
ADD CONSTRAINT "CarBooking_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "CarDocument" DROP CONSTRAINT "CarDocument_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "listingId",
ADD COLUMN     "listingId" INTEGER NOT NULL,
ADD CONSTRAINT "CarDocument_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "CarImage" DROP CONSTRAINT "CarImage_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "listingId",
ADD COLUMN     "listingId" INTEGER NOT NULL,
ADD CONSTRAINT "CarImage_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "CarListing" DROP CONSTRAINT "CarListing_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "dealershipId",
ADD COLUMN     "dealershipId" INTEGER NOT NULL,
ADD CONSTRAINT "CarListing_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "Checklist" DROP CONSTRAINT "Checklist_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
ADD CONSTRAINT "Checklist_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "Consultation" DROP CONSTRAINT "Consultation_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "consultantId",
ADD COLUMN     "consultantId" INTEGER NOT NULL,
ADD CONSTRAINT "Consultation_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "HouseBooking" DROP CONSTRAINT "HouseBooking_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "userId",
ADD COLUMN     "userId" INTEGER NOT NULL,
DROP COLUMN "listingId",
ADD COLUMN     "listingId" INTEGER NOT NULL,
ADD CONSTRAINT "HouseBooking_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "HouseImage" DROP CONSTRAINT "HouseImage_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "listingId",
ADD COLUMN     "listingId" INTEGER NOT NULL,
ADD CONSTRAINT "HouseImage_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "HouseListing" DROP CONSTRAINT "HouseListing_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "landlordId",
ADD COLUMN     "landlordId" INTEGER NOT NULL,
ADD CONSTRAINT "HouseListing_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "Payment" DROP CONSTRAINT "Payment_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "userId",
ADD COLUMN     "userId" INTEGER NOT NULL,
ADD CONSTRAINT "Payment_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "PropertyDocument" DROP CONSTRAINT "PropertyDocument_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "listingId",
ADD COLUMN     "listingId" INTEGER NOT NULL,
ADD CONSTRAINT "PropertyDocument_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "Role" DROP CONSTRAINT "Role_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
ADD CONSTRAINT "Role_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "User" DROP CONSTRAINT "User_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "roleId",
ADD COLUMN     "roleId" INTEGER NOT NULL,
ADD CONSTRAINT "User_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "UserChecklistItem" DROP CONSTRAINT "UserChecklistItem_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "userId",
ADD COLUMN     "userId" INTEGER NOT NULL,
DROP COLUMN "checklistId",
ADD COLUMN     "checklistId" INTEGER NOT NULL,
ADD CONSTRAINT "UserChecklistItem_pkey" PRIMARY KEY ("id");

-- AlterTable
ALTER TABLE "UserDocument" DROP CONSTRAINT "UserDocument_pkey",
DROP COLUMN "id",
ADD COLUMN     "id" SERIAL NOT NULL,
DROP COLUMN "userId",
ADD COLUMN     "userId" INTEGER NOT NULL,
ADD CONSTRAINT "UserDocument_pkey" PRIMARY KEY ("id");

-- AddForeignKey
ALTER TABLE "User" ADD CONSTRAINT "User_roleId_fkey" FOREIGN KEY ("roleId") REFERENCES "Role"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "HouseListing" ADD CONSTRAINT "HouseListing_landlordId_fkey" FOREIGN KEY ("landlordId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarListing" ADD CONSTRAINT "CarListing_dealershipId_fkey" FOREIGN KEY ("dealershipId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "HouseBooking" ADD CONSTRAINT "HouseBooking_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "HouseBooking" ADD CONSTRAINT "HouseBooking_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "HouseListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarBooking" ADD CONSTRAINT "CarBooking_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarBooking" ADD CONSTRAINT "CarBooking_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "CarListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "UserDocument" ADD CONSTRAINT "UserDocument_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "PropertyDocument" ADD CONSTRAINT "PropertyDocument_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "HouseListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarDocument" ADD CONSTRAINT "CarDocument_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "CarListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "UserChecklistItem" ADD CONSTRAINT "UserChecklistItem_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "UserChecklistItem" ADD CONSTRAINT "UserChecklistItem_checklistId_fkey" FOREIGN KEY ("checklistId") REFERENCES "Checklist"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "Consultation" ADD CONSTRAINT "Consultation_consultantId_fkey" FOREIGN KEY ("consultantId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "Appointment" ADD CONSTRAINT "Appointment_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "Appointment" ADD CONSTRAINT "Appointment_consultationId_fkey" FOREIGN KEY ("consultationId") REFERENCES "Consultation"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "Payment" ADD CONSTRAINT "Payment_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "HouseImage" ADD CONSTRAINT "HouseImage_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "HouseListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarImage" ADD CONSTRAINT "CarImage_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "CarListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;
````

## File: BackEnd/prisma/migrations/20250203162645_add_user_business_models/migration.sql
````sql
/*
  Warnings:

  - A unique constraint covering the columns `[phoneNo]` on the table `User` will be added. If there are existing duplicate values, this will fail.
  - Added the required column `DOB` to the `User` table without a default value. This is not possible if the table is not empty.
  - Added the required column `fullName` to the `User` table without a default value. This is not possible if the table is not empty.
  - Added the required column `phoneNo` to the `User` table without a default value. This is not possible if the table is not empty.

*/
-- CreateEnum
CREATE TYPE "StatusInCanada" AS ENUM ('STUDY_PERMIT', 'WORK_PERMIT', 'PR', 'CITIZENSHIP');

-- CreateEnum
CREATE TYPE "YearsOfExperience" AS ENUM ('ONE_TO_FIVE', 'FIVE_TO_TEN', 'TEN_PLUS');

-- CreateEnum
CREATE TYPE "WorkType" AS ENUM ('BROKERAGE', 'INDEPENDENT');

-- AlterTable
ALTER TABLE "User" ADD COLUMN     "DOB" TIMESTAMP(3) NOT NULL,
ADD COLUMN     "fullName" TEXT NOT NULL,
ADD COLUMN     "phoneNo" TEXT NOT NULL,
ADD COLUMN     "statusInCanada" "StatusInCanada";

-- CreateTable
CREATE TABLE "Realtor" (
    "id" SERIAL NOT NULL,
    "userId" INTEGER NOT NULL,
    "businessName" TEXT NOT NULL,
    "businessAddress" TEXT,
    "realEstateLicenseNumber" TEXT NOT NULL,
    "yearsOfExperience" "YearsOfExperience" NOT NULL,
    "affiliatedAssociations" TEXT,
    "areasCovered" TEXT[],
    "specialties" TEXT[],
    "portfolioWebsite" TEXT,
    "businessRegistration" TEXT NOT NULL,
    "workType" "WorkType" NOT NULL,
    "brokerageName" TEXT,
    "officeLocationAvailable" BOOLEAN NOT NULL,
    "officeAddress" TEXT NOT NULL,
    "teamMembers" INTEGER NOT NULL,
    "virtualPropertyTour" BOOLEAN NOT NULL,

    CONSTRAINT "Realtor_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "CarDealership" (
    "id" SERIAL NOT NULL,
    "userId" INTEGER NOT NULL,
    "showroomLocations" TEXT[],
    "testDrivePolicy" TEXT NOT NULL,
    "financingOptions" TEXT[],
    "tradeInAvailable" BOOLEAN NOT NULL,
    "serviceWarrantyInfo" TEXT NOT NULL,
    "businessRegistration" TEXT NOT NULL,
    "businessName" TEXT NOT NULL,
    "yearsInBusiness" "YearsOfExperience" NOT NULL,
    "dealershipLicenseNumber" TEXT NOT NULL,
    "carBrandsSold" TEXT[],
    "newOrUsedCars" TEXT[],
    "officeLocationAvailable" BOOLEAN NOT NULL,
    "officeAddress" TEXT,

    CONSTRAINT "CarDealership_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "ImmigrationConsultant" (
    "id" SERIAL NOT NULL,
    "userId" INTEGER NOT NULL,
    "countriesServed" TEXT[],
    "consultationFee" DOUBLE PRECISION,
    "businessRegistration" TEXT NOT NULL,
    "partneredLegalFirms" TEXT,
    "websiteOrSocialMedia" TEXT,
    "businessName" TEXT NOT NULL,
    "businessAddress" TEXT NOT NULL,
    "yearsOfExperience" "YearsOfExperience" NOT NULL,
    "licenseNumber" TEXT NOT NULL,
    "servicesOffered" TEXT[],
    "languagesSpoken" TEXT[],

    CONSTRAINT "ImmigrationConsultant_pkey" PRIMARY KEY ("id")
);

-- CreateIndex
CREATE UNIQUE INDEX "Realtor_userId_key" ON "Realtor"("userId");

-- CreateIndex
CREATE UNIQUE INDEX "CarDealership_userId_key" ON "CarDealership"("userId");

-- CreateIndex
CREATE UNIQUE INDEX "ImmigrationConsultant_userId_key" ON "ImmigrationConsultant"("userId");

-- CreateIndex
CREATE UNIQUE INDEX "User_phoneNo_key" ON "User"("phoneNo");

-- AddForeignKey
ALTER TABLE "Realtor" ADD CONSTRAINT "Realtor_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "CarDealership" ADD CONSTRAINT "CarDealership_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "ImmigrationConsultant" ADD CONSTRAINT "ImmigrationConsultant_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;
````

## File: BackEnd/prisma/migrations/20250203185734_changed/migration.sql
````sql
/*
  Warnings:

  - Changed the type of `yearsInBusiness` on the `CarDealership` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `yearsOfExperience` on the `ImmigrationConsultant` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.
  - Changed the type of `yearsOfExperience` on the `Realtor` table. No cast exists, the column would be dropped and recreated, which cannot be done if there is data, since the column is required.

*/
-- AlterTable
ALTER TABLE "CarDealership" DROP COLUMN "yearsInBusiness",
ADD COLUMN     "yearsInBusiness" TEXT NOT NULL;

-- AlterTable
ALTER TABLE "ImmigrationConsultant" DROP COLUMN "yearsOfExperience",
ADD COLUMN     "yearsOfExperience" TEXT NOT NULL;

-- AlterTable
ALTER TABLE "Realtor" DROP COLUMN "yearsOfExperience",
ADD COLUMN     "yearsOfExperience" TEXT NOT NULL;

-- DropEnum
DROP TYPE "YearsOfExperience";
````

## File: BackEnd/prisma/migrations/20250203190329_added/migration.sql
````sql
-- AlterTable
ALTER TABLE "Realtor" ALTER COLUMN "officeAddress" DROP NOT NULL;
````

## File: BackEnd/prisma/migrations/20250206183710_added/migration.sql
````sql
-- AlterTable
ALTER TABLE "User" ADD COLUMN     "userVerified" BOOLEAN DEFAULT false;
````

## File: BackEnd/prisma/migrations/20250207191540_added/migration.sql
````sql
-- AlterTable
ALTER TABLE "User" ADD COLUMN     "backgroundVerification" BOOLEAN DEFAULT false,
ADD COLUMN     "termsConditionCheck" BOOLEAN DEFAULT false;
````

## File: BackEnd/prisma/migrations/20250209223549_removed/migration.sql
````sql
/*
  Warnings:

  - You are about to drop the column `officeAddress` on the `CarDealership` table. All the data in the column will be lost.
  - You are about to drop the column `officeLocationAvailable` on the `CarDealership` table. All the data in the column will be lost.
  - You are about to drop the column `officeAddress` on the `Realtor` table. All the data in the column will be lost.

*/
-- AlterTable
ALTER TABLE "CarDealership" DROP COLUMN "officeAddress",
DROP COLUMN "officeLocationAvailable";

-- AlterTable
ALTER TABLE "Realtor" DROP COLUMN "officeAddress";
````

## File: BackEnd/prisma/migrations/20250210232144_added/migration.sql
````sql
-- AlterTable
ALTER TABLE "HouseListing" ADD COLUMN     "endDate" TIMESTAMP(3),
ADD COLUMN     "endTime" TEXT,
ADD COLUMN     "openhouse" BOOLEAN NOT NULL DEFAULT false,
ADD COLUMN     "startTime" TEXT,
ADD COLUMN     "startdate" TIMESTAMP(3);
````

## File: BackEnd/prisma/migrations/20250214023231_replaced/migration.sql
````sql
-- AlterTable
ALTER TABLE "CarDealership" ALTER COLUMN "showroomLocations" SET NOT NULL,
ALTER COLUMN "showroomLocations" SET DATA TYPE TEXT,
ALTER COLUMN "financingOptions" SET NOT NULL,
ALTER COLUMN "financingOptions" SET DATA TYPE TEXT,
ALTER COLUMN "carBrandsSold" SET NOT NULL,
ALTER COLUMN "carBrandsSold" SET DATA TYPE TEXT,
ALTER COLUMN "newOrUsedCars" SET NOT NULL,
ALTER COLUMN "newOrUsedCars" SET DATA TYPE TEXT;

-- AlterTable
ALTER TABLE "ImmigrationConsultant" ALTER COLUMN "countriesServed" SET NOT NULL,
ALTER COLUMN "countriesServed" SET DATA TYPE TEXT,
ALTER COLUMN "servicesOffered" SET NOT NULL,
ALTER COLUMN "servicesOffered" SET DATA TYPE TEXT,
ALTER COLUMN "languagesSpoken" SET NOT NULL,
ALTER COLUMN "languagesSpoken" SET DATA TYPE TEXT;

-- AlterTable
ALTER TABLE "Realtor" ALTER COLUMN "areasCovered" SET NOT NULL,
ALTER COLUMN "areasCovered" SET DATA TYPE TEXT,
ALTER COLUMN "specialties" SET NOT NULL,
ALTER COLUMN "specialties" SET DATA TYPE TEXT;
````

## File: BackEnd/prisma/migrations/20250214234943_updated/migration.sql
````sql
/*
  Warnings:

  - The `statusInCanada` column on the `User` table would be dropped and recreated. This will lead to data loss if there is data in the column.

*/
-- AlterTable
ALTER TABLE "User" DROP COLUMN "statusInCanada",
ADD COLUMN     "statusInCanada" TEXT;

-- DropEnum
DROP TYPE "StatusInCanada";
````

## File: BackEnd/prisma/migrations/20250304180920_updated/migration.sql
````sql
-- AlterTable
ALTER TABLE "CarListing" ADD COLUMN     "exteriorColor" TEXT,
ADD COLUMN     "fuelType" TEXT,
ADD COLUMN     "interiorColor" TEXT,
ADD COLUMN     "mileage" INTEGER,
ADD COLUMN     "noOfSeats" INTEGER,
ADD COLUMN     "status" TEXT,
ADD COLUMN     "transmission" TEXT,
ADD COLUMN     "vehicleType" TEXT,
ADD COLUMN     "vin" TEXT,
ADD COLUMN     "year" INTEGER;

-- AlterTable
ALTER TABLE "HouseListing" ADD COLUMN     "bathrooms" INTEGER,
ADD COLUMN     "bedrooms" INTEGER,
ADD COLUMN     "squareFeet" INTEGER;
````

## File: BackEnd/prisma/migrations/20250310210628_removed/migration.sql
````sql
/*
  Warnings:

  - You are about to drop the `Checklist` table. If the table is not empty, all the data it contains will be lost.
  - You are about to drop the `UserChecklistItem` table. If the table is not empty, all the data it contains will be lost.
  - Added the required column `updatedAt` to the `CarBooking` table without a default value. This is not possible if the table is not empty.

*/
-- DropForeignKey
ALTER TABLE "UserChecklistItem" DROP CONSTRAINT "UserChecklistItem_checklistId_fkey";

-- DropForeignKey
ALTER TABLE "UserChecklistItem" DROP CONSTRAINT "UserChecklistItem_userId_fkey";

-- AlterTable
ALTER TABLE "CarBooking" ADD COLUMN     "meetLink" TEXT,
ADD COLUMN     "updatedAt" TIMESTAMP(3) NOT NULL;

-- AlterTable
ALTER TABLE "HouseBooking" ADD COLUMN     "meetLink" TEXT;

-- DropTable
DROP TABLE "Checklist";

-- DropTable
DROP TABLE "UserChecklistItem";

-- CreateTable
CREATE TABLE "Availability" (
    "id" SERIAL NOT NULL,
    "userId" INTEGER NOT NULL,
    "listingType" TEXT,
    "ListingId" INTEGER,
    "startTime" TIMESTAMP(3) NOT NULL,
    "endTime" TIMESTAMP(3) NOT NULL,
    "status" TEXT NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "Availability_pkey" PRIMARY KEY ("id")
);

-- AddForeignKey
ALTER TABLE "Availability" ADD CONSTRAINT "Availability_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;
````

## File: BackEnd/prisma/migrations/20250311153000_adjusted/migration.sql
````sql
/*
  Warnings:

  - You are about to drop the column `ListingId` on the `Availability` table. All the data in the column will be lost.
  - You are about to drop the column `listingType` on the `Availability` table. All the data in the column will be lost.
  - You are about to drop the column `updatedAt` on the `CarBooking` table. All the data in the column will be lost.

*/
-- AlterTable
ALTER TABLE "Availability" DROP COLUMN "ListingId",
DROP COLUMN "listingType";

-- AlterTable
ALTER TABLE "CarBooking" DROP COLUMN "updatedAt";
````

## File: BackEnd/prisma/migrations/20250314193459_adjusted/migration.sql
````sql
-- AlterTable
ALTER TABLE "User" ADD COLUMN     "googleRefreshToken" TEXT;
````

## File: BackEnd/prisma/migrations/20250322164348_created/migration.sql
````sql
/*
  Warnings:

  - You are about to drop the `Appointment` table. If the table is not empty, all the data it contains will be lost.
  - You are about to drop the `Consultation` table. If the table is not empty, all the data it contains will be lost.

*/
-- DropForeignKey
ALTER TABLE "Appointment" DROP CONSTRAINT "Appointment_consultationId_fkey";

-- DropForeignKey
ALTER TABLE "Appointment" DROP CONSTRAINT "Appointment_userId_fkey";

-- DropForeignKey
ALTER TABLE "Consultation" DROP CONSTRAINT "Consultation_consultantId_fkey";

-- DropTable
DROP TABLE "Appointment";

-- DropTable
DROP TABLE "Consultation";

-- CreateTable
CREATE TABLE "ConsultationBooking" (
    "id" SERIAL NOT NULL,
    "userId" INTEGER NOT NULL,
    "statusInCanada" TEXT NOT NULL,
    "startDate" TIMESTAMP(3) NOT NULL,
    "endDate" TIMESTAMP(3) NOT NULL,
    "status" TEXT NOT NULL,
    "meetLink" TEXT,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,
    "consultantId" INTEGER NOT NULL,

    CONSTRAINT "ConsultationBooking_pkey" PRIMARY KEY ("id")
);

-- AddForeignKey
ALTER TABLE "ConsultationBooking" ADD CONSTRAINT "ConsultationBooking_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;
````

## File: BackEnd/prisma/migrations/20250322171321_updated/migration.sql
````sql
-- AlterTable
ALTER TABLE "User" ADD COLUMN     "alreadyInCanada" BOOLEAN,
ADD COLUMN     "countryOfOrigin" TEXT,
ADD COLUMN     "currentLocation" TEXT;
````

## File: BackEnd/prisma/migrations/20250322193650_updated/migration.sql
````sql
/*
  Warnings:

  - You are about to drop the column `statusInCanada` on the `ConsultationBooking` table. All the data in the column will be lost.

*/
-- AlterTable
ALTER TABLE "ConsultationBooking" DROP COLUMN "statusInCanada";
````

## File: BackEnd/prisma/migrations/20250322201228_updated/migration.sql
````sql
-- AddForeignKey
ALTER TABLE "ConsultationBooking" ADD CONSTRAINT "ConsultationBooking_consultantId_fkey" FOREIGN KEY ("consultantId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;
````

## File: BackEnd/prisma/migrations/20250401163908_favourite/migration.sql
````sql
-- CreateTable
CREATE TABLE "FavouriteCar" (
    "id" SERIAL NOT NULL,
    "userId" INTEGER NOT NULL,
    "listingId" INTEGER NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "FavouriteCar_pkey" PRIMARY KEY ("id")
);

-- CreateTable
CREATE TABLE "FavouriteHouse" (
    "id" SERIAL NOT NULL,
    "userId" INTEGER NOT NULL,
    "listingId" INTEGER NOT NULL,
    "createdAt" TIMESTAMP(3) NOT NULL DEFAULT CURRENT_TIMESTAMP,

    CONSTRAINT "FavouriteHouse_pkey" PRIMARY KEY ("id")
);

-- CreateIndex
CREATE UNIQUE INDEX "FavouriteCar_userId_listingId_key" ON "FavouriteCar"("userId", "listingId");

-- CreateIndex
CREATE UNIQUE INDEX "FavouriteHouse_userId_listingId_key" ON "FavouriteHouse"("userId", "listingId");

-- AddForeignKey
ALTER TABLE "FavouriteCar" ADD CONSTRAINT "FavouriteCar_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "FavouriteCar" ADD CONSTRAINT "FavouriteCar_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "CarListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "FavouriteHouse" ADD CONSTRAINT "FavouriteHouse_userId_fkey" FOREIGN KEY ("userId") REFERENCES "User"("id") ON DELETE RESTRICT ON UPDATE CASCADE;

-- AddForeignKey
ALTER TABLE "FavouriteHouse" ADD CONSTRAINT "FavouriteHouse_listingId_fkey" FOREIGN KEY ("listingId") REFERENCES "HouseListing"("id") ON DELETE RESTRICT ON UPDATE CASCADE;
````

## File: BackEnd/prisma/migrations/migration_lock.toml
````toml
# Please do not edit this file manually
# It should be added in your version-control system (e.g., Git)
provider = "postgresql"
````

## File: BackEnd/prisma/schema.prisma
````
generator client {
  provider = "prisma-client-js"
}

datasource db {
  provider = "postgresql"
  url      = env("DATABASE_URL")
}

model User {
  email                  String                 @unique
  firebaseUid            String                 @unique
  createdAt              DateTime               @default(now())
  id                     Int                    @id @default(autoincrement())
  roleId                 Int
  DOB                    DateTime
  fullName               String
  phoneNo                String                 @unique
  userVerified           Boolean?               @default(false)
  backgroundVerification Boolean?               @default(false)
  termsConditionCheck    Boolean?               @default(false)
  statusInCanada         String?
  googleRefreshToken     String?
  alreadyInCanada        Boolean?
  countryOfOrigin        String?
  currentLocation        String?
  availableSlots         Availability[]
  carBookings            CarBooking[]
  carDealership          CarDealership?
  carListings            CarListing[]
  consultantSessions     ConsultationBooking[]  @relation("Consultant")
  consultationBookings   ConsultationBooking[]  @relation("User")
  favouriteCars          FavouriteCar[]
  favouriteHouses        FavouriteHouse[]
  houseBookings          HouseBooking[]
  houseListings          HouseListing[]
  immigrationConsultant  ImmigrationConsultant?
  payments               Payment[]
  realtor                Realtor?
  role                   Role                   @relation(fields: [roleId], references: [id])
  userDocuments          UserDocument[]
}

model Realtor {
  id                      Int      @id @default(autoincrement())
  userId                  Int      @unique
  businessName            String
  businessAddress         String?
  realEstateLicenseNumber String
  affiliatedAssociations  String?
  areasCovered            String
  specialties             String
  portfolioWebsite        String?
  businessRegistration    String
  workType                WorkType
  brokerageName           String?
  officeLocationAvailable Boolean
  teamMembers             Int
  virtualPropertyTour     Boolean
  yearsOfExperience       String
  user                    User     @relation(fields: [userId], references: [id])
}

model CarDealership {
  id                      Int     @id @default(autoincrement())
  userId                  Int     @unique
  showroomLocations       String
  testDrivePolicy         String
  financingOptions        String
  tradeInAvailable        Boolean
  serviceWarrantyInfo     String
  businessRegistration    String
  businessName            String
  dealershipLicenseNumber String
  carBrandsSold           String
  newOrUsedCars           String
  yearsInBusiness         String
  user                    User    @relation(fields: [userId], references: [id])
}

model ImmigrationConsultant {
  id                   Int     @id @default(autoincrement())
  userId               Int     @unique
  countriesServed      String
  consultationFee      Float?
  businessRegistration String
  partneredLegalFirms  String?
  websiteOrSocialMedia String?
  businessName         String
  businessAddress      String
  licenseNumber        String
  servicesOffered      String
  languagesSpoken      String
  yearsOfExperience    String
  user                 User    @relation(fields: [userId], references: [id])
}

model Role {
  name  String @unique
  id    Int    @id @default(autoincrement())
  users User[]
}

model HouseListing {
  title         String
  description   String?
  price         Decimal
  location      String
  createdAt     DateTime           @default(now())
  id            Int                @id @default(autoincrement())
  landlordId    Int
  endDate       DateTime?
  endTime       String?
  openhouse     Boolean            @default(false)
  startTime     String?
  startdate     DateTime?
  bathrooms     Int?
  bedrooms      Int?
  squareFeet    Int?
  favourites    FavouriteHouse[]
  houseBookings HouseBooking[]
  houseImages   HouseImage[]
  landlord      User               @relation(fields: [landlordId], references: [id])
  propertyDocs  PropertyDocument[]
}

model CarListing {
  model         String
  make          String
  price         Decimal
  createdAt     DateTime       @default(now())
  id            Int            @id @default(autoincrement())
  dealershipId  Int
  exteriorColor String?
  fuelType      String?
  interiorColor String?
  mileage       Int?
  noOfSeats     Int?
  status        String?
  transmission  String?
  vehicleType   String?
  vin           String?
  year          Int?
  carBookings   CarBooking[]
  carDocs       CarDocument[]
  carImages     CarImage[]
  dealership    User           @relation(fields: [dealershipId], references: [id])
  favourites    FavouriteCar[]
}

model Availability {
  id        Int      @id @default(autoincrement())
  userId    Int
  startTime DateTime
  endTime   DateTime
  status    String
  createdAt DateTime @default(now())
  user      User     @relation(fields: [userId], references: [id])
}

model HouseBooking {
  startDate DateTime
  endDate   DateTime
  status    String
  createdAt DateTime     @default(now())
  id        Int          @id @default(autoincrement())
  userId    Int
  listingId Int
  meetLink  String?
  listing   HouseListing @relation(fields: [listingId], references: [id])
  user      User         @relation(fields: [userId], references: [id])
}

model CarBooking {
  startDate DateTime
  endDate   DateTime
  status    String
  createdAt DateTime   @default(now())
  id        Int        @id @default(autoincrement())
  userId    Int
  listingId Int
  meetLink  String?
  listing   CarListing @relation(fields: [listingId], references: [id])
  user      User       @relation(fields: [userId], references: [id])
}

model ConsultationBooking {
  id           Int      @id @default(autoincrement())
  userId       Int
  startDate    DateTime
  endDate      DateTime
  status       String
  meetLink     String?
  createdAt    DateTime @default(now())
  consultantId Int
  consultant   User     @relation("Consultant", fields: [consultantId], references: [id])
  user         User     @relation("User", fields: [userId], references: [id])
}

model UserDocument {
  documentType String
  fileData     Bytes
  createdAt    DateTime @default(now())
  id           Int      @id @default(autoincrement())
  userId       Int
  user         User     @relation(fields: [userId], references: [id])
}

model PropertyDocument {
  documentType String
  fileData     Bytes
  createdAt    DateTime     @default(now())
  id           Int          @id @default(autoincrement())
  listingId    Int
  listing      HouseListing @relation(fields: [listingId], references: [id])
}

model CarDocument {
  documentType String
  fileData     Bytes
  createdAt    DateTime   @default(now())
  id           Int        @id @default(autoincrement())
  listingId    Int
  listing      CarListing @relation(fields: [listingId], references: [id])
}

model Payment {
  amount          Decimal
  transactionType String
  createdAt       DateTime @default(now())
  id              Int      @id @default(autoincrement())
  userId          Int
  user            User     @relation(fields: [userId], references: [id])
}

model HouseImage {
  imageData Bytes
  createdAt DateTime     @default(now())
  id        Int          @id @default(autoincrement())
  listingId Int
  listing   HouseListing @relation(fields: [listingId], references: [id])
}

model CarImage {
  imageData Bytes
  createdAt DateTime   @default(now())
  id        Int        @id @default(autoincrement())
  listingId Int
  listing   CarListing @relation(fields: [listingId], references: [id])
}

model FavouriteCar {
  id        Int        @id @default(autoincrement())
  userId    Int
  listingId Int
  createdAt DateTime   @default(now())
  listing   CarListing @relation(fields: [listingId], references: [id])
  user      User       @relation(fields: [userId], references: [id])

  @@unique([userId, listingId])
}

model FavouriteHouse {
  id        Int          @id @default(autoincrement())
  userId    Int
  listingId Int
  createdAt DateTime     @default(now())
  listing   HouseListing @relation(fields: [listingId], references: [id])
  user      User         @relation(fields: [userId], references: [id])

  @@unique([userId, listingId], name: "userId_listingId")
}

enum WorkType {
  BROKERAGE
  INDEPENDENT
}
````

## File: BackEnd/prisma/seed.js
````javascript
const { PrismaClient } = require('@prisma/client');


const prisma = new PrismaClient();

async function main() {
  // Create Roles
  const immigrantRole = await prisma.role.create({
    data: {
      name: 'Immigrant',
    },
  });
  const realtorRole = await prisma.role.create({
    data: {
      name: 'Realtor',
    },
  });

  const carRole = await prisma.role.create({
    data: {
      name: 'Car Dealership',
    },
  });

  const consultantRole = await prisma.role.create({
    data: {
      name: 'Immigration Consultant',
    },
  });





}
main()
  .catch((e) => {
    console.error(e);
    process.exit(1);
  })
  .finally(async () => {
    await prisma.$disconnect();
  });
````

## File: BackEnd/README.md
````markdown
# ImmigrateX-BackEnd
This is backend Repo
````

## File: BackEnd/routes/admin/adminStatsRoute.js
````javascript
const express = require('express');
const verifyToken = require('../../middleware/authMiddleware');
const { PrismaClient } = require('@prisma/client');

const prisma = new PrismaClient();

const statsRouter = express.Router();

statsRouter.get('/stats', async (req, res) => {
    try {
        // Total users count
        const totalUsers = await prisma.user.count();

        // Verified and unverified users count
        const verifiedUsers = await prisma.user.count({ where: { userVerified: true } });
        const unverifiedUsers = totalUsers - verifiedUsers;

        const noOfImmigrant = await prisma.user.count({ where: { roleId: 1 } });

        const usersByMonth = await prisma.user.findMany({
            select: {
                createdAt: true
            }
        });
    
        // Group data by month
        const monthlyCounts = usersByMonth.reduce((acc, user) => {
            const month = new Date(user.createdAt).toLocaleString('default', { month: 'short', year: 'numeric' });
            acc[month] = (acc[month] || 0) + 1;
            return acc;
        }, {});
    
        // Convert to array format
        const formattedData = Object.entries(monthlyCounts).map(([month, count]) => ({
            month,
            count
        }));

        // Total house and car listings
        const houseListings = await prisma.houseListing.count();
        const carListings = await prisma.carListing.count();

        // User type distribution (bar graph)
        const userTypes = await prisma.user.groupBy({
            by: ['roleId'],
            _count: { id: true }
        });

        // Fetch role names based on roleId
        const roles = await prisma.role.findMany();
        const roleMap = Object.fromEntries(roles.map(role => [role.id, role.name]));

        // Format user type graph data
        const userTypeGraph = userTypes.map(type => ({
            userType: roleMap[type.roleId] || 'Unknown',
            count: type._count.id
        }));

        res.json({
            totalUsers,
            verifiedUsers,
            unverifiedUsers,
            formattedData,
            noOfImmigrant,
            houseListings,
            carListings,
            userTypeGraph,
            verificationPieChart: [
                { label: 'Verified', value: verifiedUsers },
                { label: 'Unverified', value: unverifiedUsers }
            ]
        });
    } catch (error) {
        console.error('Error fetching dashboard data:', error);
        res.status(500).json({ error: 'Internal server error' });
    } finally {
        await prisma.$disconnect();
    }
});

module.exports = statsRouter;
````

## File: BackEnd/routes/admin/userDetailsRoute.js
````javascript
const express = require('express');
const verifyToken = require('../../middleware/authMiddleware');
const { PrismaClient } = require('@prisma/client');

const prisma = new PrismaClient();

const userDetailRouter = express.Router();


userDetailRouter.get("/user-details",verifyToken, async (req, res) => {
    
    try {
      
       
          const user = await prisma.user.findMany({
            where: {
              roleId: {
                not: 5,
              },
            },
            select: {
              id: true,
              fullName: true,
              email: true,
              phoneNo: true,
              DOB: true,
              firebaseUid: true,
              userVerified: true,
              statusInCanada: true,
              roleId: true,
              userDocuments: {
                select: {
                  id: true, // Fetch only the document ID
                },
              },
            },
          });
          
          
        if (!user || user.length === 0) {
            return res.status(404).json({ error: 'No users found' });
          }
  
      res.status(200).json({user});
    } catch (error) {
      console.log(error.message);
      res.status(400).json({ error: error.message });
    }
  });

  
userDetailRouter.get("/user-details/:userId",verifyToken, async (req, res) => {
    
  try {
    
      const user = await prisma.user.findUnique({
        where:{
          id:parseInt(req.params.userId)
        },
        include: {
          realtor: true,
          carDealership: true,
          immigrationConsultant: true,
          userDocuments: {
            select:{
              id:true
            }
          }
        }
        });
        
        
      if (!user || user.length === 0) {
          return res.status(404).json({ error: 'No users found' });
        }

    res.status(200).json({user});
  } catch (error) {
    console.log(error.message);
    res.status(400).json({ error: error.message });
  }
});

userDetailRouter.get("/user-document/:documentId",verifyToken, async (req, res) => {
    
  try {
    const documentId = parseInt(req.params.documentId, 10);
    if (isNaN(documentId)) {
        return res.status(400).json({ error: "Invalid document ID" });
    }
  
    const document = await prisma.userDocument.findUnique({
        where: { id: documentId },
        select: {
            fileData: true, // File stored as BLOB (Bytes)
            documentType: true,
        },
    });
  
    if (!document) {
        return res.status(404).json({ error: "Document not found" });
    }
  
    // Convert BLOB to Buffer
    const pdfBuffer = Buffer.from(document.fileData);
  
    // Set response headers for PDF display in iframe
    res.setHeader("Content-Type", "application/pdf");
    res.setHeader("Content-Disposition", "inline"); // View in browser/iframe
    res.send(pdfBuffer);
  } catch (error) {
    console.error("Error fetching document:", error);
    res.status(500).json({ error: "Internal server error" });
  }
});



  module.exports = userDetailRouter;
````

## File: BackEnd/routes/admin/verifyUserRoute.js
````javascript
const express = require('express');
const verifyToken = require('../../middleware/authMiddleware');
const { PrismaClient } = require('@prisma/client');

const prisma = new PrismaClient();

const verifyUserRouter = express.Router();


verifyUserRouter.get("/unverified-user",verifyToken, async (req, res) => {
    
    try {
      
      const user = await prisma.user.findMany({
        where: {
          userVerified: false,
          roleId: {
            not: 5,
          },
        },
        select: {
          id: true,
          fullName: true,
          email: true,
          phoneNo: true,
          DOB: true,
          firebaseUid: true,
          userVerified: true,
          statusInCanada: true,
          roleId: true,
          userDocuments: {
            select: {
              id: true, // Fetch only the document ID
            },
          },
        },
      });
      
          
          
        if (!user || user.length === 0) {
            return res.status(404).json({ error: 'No users found' });
          }
  
      res.status(200).json({user});
    } catch (error) {
      console.log(error.message);
      res.status(400).json({ error: error.message });
    }
  });

verifyUserRouter.put("/verify-user",verifyToken, async (req, res) => {
  
    try {

        const updatedUser = await prisma.user.update({
            where: { id: req.body.id },
            data: {
              userVerified:true,
            }
          });

          // @manpreet - add send documents verified email here ..get email id from req.body.email
  
      res.status(200).json({ updatedUser });
    } catch (error) {
      console.log(error.message);
      res.status(400).json({ error: error.message });
    }
  });

  module.exports = verifyUserRouter;
````

## File: BackEnd/routes/appointment.js
````javascript
const express = require('express');
const { google } = require('googleapis');
const verifyToken = require('../middleware/authMiddleware');
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();
const { getAccessToken } = require('../middleware/oauthTokenMiddleware');
const appointmentRouter = express.Router();

const convertToUserTimezone = (utcDate, userTimezone) => {
    const date = new Date(utcDate);
    if (isNaN(date.getTime())) return "Invalid Date"; // Prevents errors
  
    return date.toISOString(); // Returns valid ISO 8601 format
  };
// Function to Schedule Google Calendar Event
async function scheduleEvent(accessToken, userEmail, attendeesEmails, startTime, endTime, title) {
    const auth = new google.auth.OAuth2();
    auth.setCredentials({ access_token: accessToken });

    const calendar = google.calendar({ version: 'v3', auth });

   

    const event = {
        summary: title,
        description: 'Appointment scheduled via platform',
        start: { dateTime: startTime.toISOString(), timeZone: 'UTC' },
        end: { dateTime: endTime.toISOString(), timeZone: 'UTC' },
        attendees: [
            { email: userEmail }, // Add the current user
            {email: attendeesEmails} // Add all attendees
        ],
        conferenceData: {
            createRequest: {
                requestId: `meet-${Date.now()}`,
                conferenceSolutionKey: { type: 'hangoutsMeet' }
            }
        }
    };

    try {
        const response = await calendar.events.insert({
            calendarId: 'primary',
            resource: event,
            conferenceDataVersion: 1,
            sendUpdates: "all" // Ensures attendees receive email notifications
        });

        return response.data;
    } catch (error) {
        console.error('Error creating event:', error);
        throw new Error({ message: "Failed to schedule event", error: error.message });
    }
}

// API Endpoint to Schedule an Appointment
appointmentRouter.post('/schedule', verifyToken, async (req, res) => {
    try {
        const listingId = parseInt(req.body.listingId);
        const availabilityId = parseInt(req.body.availabilityId);

        // Fetch the availability record from the database
        const availability = await prisma.availability.findUnique({
            where: { id: availabilityId },
            include: { user: { include: { role: true } } }
        });

        if (!availability) {
            return res.status(404).json({ error: 'Availability not found' });
        }

        const user = await prisma.user.findUnique({ where: { email: req.user.email } });
        if (!user) {
            return res.status(404).json({ error: 'User not found' });
        }

        if (!user.googleRefreshToken) {
            return res.status(403).json({
                error: "Google Calendar access required. Please connect your Google account.",
                connectUrl: 'http://localhost:5500/api/protected/oauth/auth/google'
            });
        }

        // Extract Start and End Time from the availability object
        const startTime = availability.startTime; // Ensure this field exists in your DB
        const endTime = availability.endTime; // Ensure this field exists in your DB

        if (!startTime || !endTime) {
            return res.status(400).json({ error: 'Invalid availability data: Missing start or end time.' });
        }

        // Get Access Token from Refresh Token
        const accessToken = await getAccessToken(user.googleRefreshToken);
        const title = "Meeting with " + availability.user.role.name;

        // Schedule the event with attendees
        const event = await scheduleEvent(accessToken, req.user.email, availability.user.email, startTime, endTime, title);

        let appointment;
        if (availability.user.role.name === "Realtor") {
            appointment = await prisma.HouseBooking.create({
                data: { userId: user.id, listingId, startDate: startTime, endDate: endTime, status: "Confirmed", meetLink: event.hangoutLink }
            });
        } else if (availability.user.role.name === "Car Dealership") {
            appointment = await prisma.CarBooking.create({
                data: { userId: user.id, listingId, startDate: startTime, endDate: endTime, status: "Confirmed", meetLink: event.hangoutLink }
            });
        }else if (availability.user.role.name === "Immigration Consultant") {
          appointment = await prisma.ConsultationBooking.create({
              data: { userId: user.id, startDate: startTime, endDate: endTime, status: "Confirmed", meetLink: event.hangoutLink, consultantId: listingId }
          });
      }


        await prisma.availability.update({
            where: { id : availabilityId },
            data: { status: "Booked" }
        });

        return res.status(201).json({ message: 'Event scheduled', appointment });

    } catch (error) {
        console.error("Error scheduling appointment:", error);
        return res.status(500).json({ error: error.message });
    }
});


appointmentRouter.get("/user-info", verifyToken, async (req, res) => {
  try {
    const user = await prisma.user.findUnique({
      where: { email: req.user.email },
      include: { role: true }
    });

    if (!user) return res.status(404).json({ error: "User not found" });


    const userTimezone = Intl.DateTimeFormat().resolvedOptions().timeZone;

    // Fetch house bookings with user details
    const houseBookings = await prisma.houseBooking.findMany({
      where: { listing: { landlordId: user.id }, status: "Confirmed" },
      include: { 
        listing: true,
        user: true // Fetch user who made the booking
      }
    });

    // Fetch car bookings with user details
    const carBookings = await prisma.CarBooking.findMany({
      where: { listing: { dealershipId: user.id }, status: "Confirmed" },
      include: { 
        listing: true,
        user: true // Fetch user who made the booking
      }
    });

    const consultationBookings = await prisma.ConsultationBooking.findMany({
      where: { consultantId: user.id, status: "Confirmed" },
      include: { 
        user: true // Fetch user who made the booking
      }
    });

    // Format house bookings with user details
    const formattedHouseBookings = houseBookings.map((slot) => ({
      id: slot.id,
      user: {
        id: slot.user.id,
        fullName: slot.user.fullName,
        email: slot.user.email,
        phoneNo: slot.user.phoneNo,
      },
      listing: {
        id: slot.listing.id,
        title: slot.listing.title,
        price: slot.listing.price,
        location: slot.listing.location
      },
      startDate: convertToUserTimezone(slot.startDate, userTimezone),
      endDate: convertToUserTimezone(slot.endDate, userTimezone),
      status: slot.status,
      meetLink: slot.meetLink || null,
      createdAt: convertToUserTimezone(slot.createdAt, userTimezone),
    }));

    // Format car bookings with user details
    const formattedCarBookings = carBookings.map((slot) => ({
      id: slot.id,
      user: {
        id: slot.user.id,
        fullName: slot.user.fullName,
        email: slot.user.email,
        phoneNo: slot.user.phoneNo,
      },
      listing: {
        id: slot.listing.id,
        make: slot.listing.make,
        model: slot.listing.model,
        price: slot.listing.price,
        year: slot.listing.year
      },
      startDate: convertToUserTimezone(slot.startDate, userTimezone),
      endDate: convertToUserTimezone(slot.endDate, userTimezone),
      status: slot.status,
      meetLink: slot.meetLink || null,
      createdAt: convertToUserTimezone(slot.createdAt, userTimezone),
    }));

    const formattedConsultationBookings = consultationBookings.map((slot) => ({
      id: slot.id,
      user: {
        id: slot.user.id,
        fullName: slot.user.fullName,
        email: slot.user.email,
        phoneNo: slot.user.phoneNo,
      },
      startDate: convertToUserTimezone(slot.startDate, userTimezone),
      endDate: convertToUserTimezone(slot.endDate, userTimezone),
      status: slot.status,
      meetLink: slot.meetLink || null,
      createdAt: convertToUserTimezone(slot.createdAt, userTimezone),
    }));

    // Structure the response
    const response = {
      success: true,

      houseBookings: formattedHouseBookings,
      carBookings: formattedCarBookings,
      icBookings: formattedConsultationBookings
    };

    res.json(response);
  } catch (error) {
    console.error("Error fetching user info:", error);
    res.status(500).json({ error: "Error fetching user info" });
  }
});

appointmentRouter.get("/view-booking", verifyToken, async (req, res) => {
  try {
    const user = await prisma.user.findUnique({
      where: { email: req.user.email },
      include: { role: true }
    });

    if (!user) return res.status(404).json({ error: "User not found" });

    const userTimezone = Intl.DateTimeFormat().resolvedOptions().timeZone;

    // Fetch house bookings with user details
    const houseBookings = await prisma.HouseBooking.findMany({
      where: { userId: user.id, status: "Confirmed" },
      include: { 
        listing:  {
          include: { landlord: true }
        } // Fetch user who made the booking
      }
    });

    // Fetch car bookings with user details
    const carBookings = await prisma.CarBooking.findMany({
      where: { userId: user.id, status: "Confirmed" },
      include: { 
        listing: {
          include: { dealership: true }
        } // Fetch user who made the booking
      }
    });

    // Format house bookings with user details
    const formattedHouseBookings = houseBookings.map((slot) => (
      {
      id: slot.id,
      listing: {
        id: slot.listing.id,
        title: slot.listing.title,
        price: slot.listing.price,
        location: slot.listing.location,
        landlord: {
          id: slot.listing.landlord.id,
          fullName: slot.listing.landlord.fullName,
          email: slot.listing.landlord.email,
          phoneNo: slot.listing.landlord.phoneNo,
        }
      },
      startDate: convertToUserTimezone(slot.startDate, userTimezone),
      endDate: convertToUserTimezone(slot.endDate, userTimezone),
      status: slot.status,
      meetLink: slot.meetLink || null,
      createdAt: convertToUserTimezone(slot.createdAt, userTimezone),
    }));


    // Format car bookings with user details
    const formattedCarBookings = carBookings.map((slot) => ({
      id: slot.id,
      
      listing: {
        id: slot.listing.id,
        make: slot.listing.make,
        model: slot.listing.model,
        price: slot.listing.price,
        year: slot.listing.year,
        dealership: {
          id: slot.listing.dealership.id,
          fullName: slot.listing.dealership.fullName,
          email: slot.listing.dealership.email,
          phoneNo: slot.listing.dealership.phoneNo,
        }
      },
      startDate: convertToUserTimezone(slot.startDate, userTimezone),
      endDate: convertToUserTimezone(slot.endDate, userTimezone),
      status: slot.status,
      meetLink: slot.meetLink || null,
      createdAt: convertToUserTimezone(slot.createdAt, userTimezone),
    }));

    // Structure the response
    const response = {
      success: true,

      houseBookings: formattedHouseBookings,
      carBookings: formattedCarBookings
    };

    res.json(response);
  } catch (error) {
    console.error("Error fetching user info:", error);
    res.status(500).json({ error: "Error fetching user info" });
  }
});

appointmentRouter.put("/complete", verifyToken, async (req, res) => {
  try {
    const { id, type } = req.body;
    
    if(type === "car"){
       await prisma.CarBooking.update({
        where: { id: parseInt(id) },
        data: {
          status: "Completed"
        },
      });
    }
    else if (type === "house"){
     await prisma.HouseBooking.update({
        where: { id: parseInt(id) },
        data: {
          status: "Completed"
        },
      });

    }
    else if (type === "consultant"){
      await prisma.ConsultationBooking.update({
         where: { id: parseInt(id) },
         data: {
           status: "Completed"
         },
       });
 
     }

   
    res.status(200).json("Updated");
  } catch (error) {
    console.error("Error updating availability:", error);
    res.status(500).json({ error: "Error updating availability" });
  }
});

appointmentRouter.get("/booking-status", verifyToken, async (req, res) => {
  try {
    console.log("sam")
    const { listingId, type } = req.query;  // Now we use req.body instead of req.query

    
    
    const user = await prisma.User.findUnique({
      where: { email: req.user.email },
    });
    console.log(req.query)

    if (!user) return res.status(404).json({ error: "User not found" });

    let booking = [];

    if (type == "car") {
      booking = await prisma.CarBooking.findMany({
        where: {
  
            listingId: parseInt(listingId),
            userId: user.id,
            status: "Confirmed",

        },
      });
    } else if (type == 'house') {
      booking = await prisma.HouseBooking.findMany({
        where: {

            listingId: parseInt(listingId),
            userId: user.id,
            status: "Confirmed",
    
        },
      });
      
    }
    else if (type == "consultant") {
      booking = await prisma.ConsultationBooking.findMany({
        select:{endDate:true},
        where: {
          consultantId: parseInt(listingId),
            userId: user.id,
            status: "Confirmed",
    
        },
      });
    }

    

    if (booking.length > 0) {
      const response = {booking: booking}
      return res.status(200).json(response);
    } else {
      return res.status(404).json("Redirect to Booking");
    }
  
  } catch (error) {
    console.error("Error checking booking status:", error);
    res.status(500).json({ error: "Error checking booking status" });
  }
});

appointmentRouter.get("/view-Cbooking", verifyToken, async (req, res) => {
  try {
    const user = await prisma.user.findUnique({
      where: { email: req.user.email },
      include: { role: true },
    });

    if (!user) return res.status(404).json({ error: "User not found" });

    const userTimezone = Intl.DateTimeFormat().resolvedOptions().timeZone;

    // Fetch consultation bookings for this user, including consultant and consultant.user info
    const consultationBookings = await prisma.consultationBooking.findMany({
      where: { userId: user.id, status: "Confirmed" },
      include: {
        consultant:true,
      },
    });

    // Format bookings
    const formattedConsultationBookings = consultationBookings.map((slot) => ({
      id: slot.id,
      consultantId: slot.consultantId,
      startDate: convertToUserTimezone(slot.startDate, userTimezone),
      endDate: convertToUserTimezone(slot.endDate, userTimezone),
      createdAt: convertToUserTimezone(slot.createdAt, userTimezone),
      status: slot.status,
      meetLink: slot.meetLink || null,
      consultant: {
       
          fullName: slot.consultant.fullName,
          email: slot.consultant.email,
          phoneNo: slot.consultant.phoneNo,
        },
    }));

    return res.json(formattedConsultationBookings,);
  } catch (error) {
    console.error("Error fetching consultation bookings:", error);
    res.status(500).json({ error: "Error fetching consultation bookings" });
  }
});




module.exports = appointmentRouter;
````

## File: BackEnd/routes/authRoutes.js
````javascript
const express = require("express");
const router = express.Router();
const axios = require("axios");
require("dotenv").config(); // Load environment variables
const admin = require("../middleware/firebaseAdminMiddleware");
const decryptPasswordMiddleware = require("../middleware/decryptionMiddleware");
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();

// Firebase REST API base URL and API key
const FIREBASE_AUTH_URL = process.env.FIREBASE_AUTH_URL;
const FIREBASE_API_KEY = process.env.FIREBASE_API_KEY;


// Helper function for Firebase API interaction
const firebaseRequest = async (url, data) => {
  try {
    const response = await axios.post(`${FIREBASE_AUTH_URL}:${url}?key=${FIREBASE_API_KEY}`, data);
    return response.data;
  } catch (error) {
    throw error.response?.data?.error || { message: "An unknown error occurred." };
  }
};

// **Routes**


// Register User with Email Verification
router.post("/signup", decryptPasswordMiddleware, async (req, res) => {
  const { email, password } = req.body;

  if (!email || !password) {
    return res.status(400).json({ error: "Email and password are required" });
  }

  try {
    // Sign up the user
    const result = await firebaseRequest("signUp", {
      email,
      password,
      returnSecureToken: true,
    });
    //console.log(result)

    // Send email verification
    const idToken = result.idToken;
   

    await firebaseRequest("sendOobCode", {
      requestType: "VERIFY_EMAIL",
      idToken,
    });

    res.cookie("refreshtoken", result.refreshToken, {
      httpOnly: true,  // Prevent access via JavaScript
      secure: process.env.NODE_ENV === "production", // Use HTTPS in production
      sameSite: "Strict", // CSRF protection
      maxAge: 7 * 24 * 60 * 60 * 1000 // 7 days expiration or 1 day
    });

    res.status(200).json({
      message: "User registered successfully. A verification email has been sent to your email address.",
      userId: result.localId,
    });
  } catch (error) {
    res.status(400).json({
      error: error.message,
    });
  }
});


// Resend Email Verification
router.post("/resend-verification", async (req, res) => {
  const idToken = req.headers.authorization?.split("Bearer ")[1]; // Extract token


  if (!idToken) {
    return res.status(400).json({ error: "ID Token is required" });
  }

  try {
    // Send a verification email
    await firebaseRequest("sendOobCode", {
      requestType: "VERIFY_EMAIL",
      idToken,
    });

    res.status(200).json({ message: "Verification email resent successfully." });
  } catch (error) {
    console.log(error.message);
    res.status(400).json({ error: error.message });
  }
});


// Login User with Email Verification Check
router.post("/login", decryptPasswordMiddleware, async (req, res) => {
  const { email, password, rememberMe } = req.body;

  if (!email || !password) {
    return res.status(400).json({ error: "Email and password are required" });
  }

  try {
    // Authenticate user
    const result = await firebaseRequest("signInWithPassword", {
      email,
      password,
      returnSecureToken: true,
    });
 
    const decodedToken = await admin.auth().verifyIdToken(result.idToken);

    // Check if the user's email is verified
    if (!decodedToken.email_verified) {
      return res.status(403).json({
        error: "Email not verified. Please verify your email before logging in.",
        emailVerified: decodedToken.email_verified,
        token: result.idToken
      });

      // if email verified check for user verified if user too - send role in reponse body for dashboard redirect else send useVerired  - false
    }
    else{

      const user = await prisma.user.findUnique({
        where: { email: decodedToken.email,
          
         },
         include: {
           role: true, 
         }
      });

      res.cookie("token", result.idToken, {
        httpOnly: true,  // Prevent access via JavaScript
        secure: process.env.NODE_ENV === "production", // Use HTTPS in production
        sameSite: "Strict", // CSRF protection
        maxAge: rememberMe ? 7 * 24 * 60 * 60 * 1000 : 24 * 60 * 60 * 1000, // 7 days expiration or 1 day
      });
      res.cookie("refreshtoken", result.refreshToken, {
        httpOnly: true,  // Prevent access via JavaScript
        secure: process.env.NODE_ENV === "production", // Use HTTPS in production
        sameSite: "Strict", // CSRF protection
        maxAge: rememberMe ? 7 * 24 * 60 * 60 * 1000 : 24 * 60 * 60 * 1000, // 7 days expiration or 1 day
      });
    
      if (user === null) {
        res.status(200).json({
          message: "Login successful",
          email: result.email,
          emailVerified: decodedToken.email_verified,
          onboarded: false
        });
      }
      else{
        if(decodedToken.email_verified && user.userVerified){
          res.status(200).json({
            message: "Login successful",
            email: result.email,
            emailVerified: decodedToken.email_verified,
            userVerified: user.userVerified,
            userRole:user.role.name,
          });
        }
        else{
          res.status(200).json({
            message: "Login successful",
            email: result.email,
            emailVerified: decodedToken.email_verified,
            userVerified: user.userVerified,
          });
        }
      }

     
    }
    
  } catch (error) {
    console.error("Login failed:", error);
    res.status(400).json({ error: error.message });
  }
});

router.post("/refresh-token", async (req, res) => {
  const refreshToken = req.cookies.refreshtoken;

  if (!refreshToken) {
    return res.status(401).json({ error: "No refresh token found. Please log in again." });
  }

  console.log("Received refresh token:", refreshToken);  // Log the token for debugging

  try {
    const response = await fetch(`https://securetoken.googleapis.com/v1/token?key=${FIREBASE_API_KEY}`, {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify({
        grant_type: "refresh_token",
        refresh_token: refreshToken,
      }),
    });

    const data = await response.json();

    console.log(data)

    if (!response.ok) {
      // Firebase returned an error, pass it to the client
      return res.status(400).json({ error: "Failed to refresh token", details: data });
    }

    // If the refresh was successful, send the new token as a cookie
    res.cookie("token", data.id_token, {
      httpOnly: true, // Prevent access via JavaScript
      secure: process.env.NODE_ENV === "production", // Use HTTPS in production
      sameSite: "Strict", // CSRF protection
      maxAge: 7 * 24 * 60 * 60 * 1000, // 7 days expiration
    });

    res.status(200).json({ message: "Refresh token successful" });
  } catch (error) {
    console.error("Error during token refresh:", error);
    res.status(400).json({ error: "Failed to refresh token", details: error.message });
  }
});


//logout
router.post("/logout", (req, res) => {
  res.clearCookie("refreshtoken"); // Clear refresh token cookie
  res.status(200).json({ message: "Logout successful" });
});

// Google Sign-In
router.post("/google-signin", async (req, res) => {
  const { idToken, refreshToken, rememberMe } = req.body;

  if (!idToken) {
    return res.status(400).json({ error: "Missing ID Token" });
  }

  try {
    // Verify ID token
    const decodedToken = await admin.auth().verifyIdToken(idToken);
    const { uid, email, name } = decodedToken;

    const user = await prisma.user.findUnique({
      where: { email: decodedToken.email,
       },
       include: {
         role: true, 
       }
    });

    res.cookie("token", idToken, {
      httpOnly: true,  // Prevent access via JavaScript
      secure: process.env.NODE_ENV === "production", // Use HTTPS in production
      sameSite: "Strict", // CSRF protection
      maxAge: rememberMe ? 7 * 24 * 60 * 60 * 1000 : 24 * 60 * 60 * 1000, // 7 days expiration or 1 day
    });
    res.cookie("refreshtoken", refreshToken, {
      httpOnly: true,  // Prevent access via JavaScript
      secure: process.env.NODE_ENV === "production", // Use HTTPS in production
      sameSite: "Strict", // CSRF protection
      maxAge: rememberMe ? 7 * 24 * 60 * 60 * 1000 : 24 * 60 * 60 * 1000, // 7 days expiration or 1 day
    });
    
    if (user === null) {
      res.status(200).json({
        message: "Login successful",
        email: email,
        emailVerified: decodedToken.email_verified,
        onboarded: false
      });
    }
    else{
      if(user.userVerified){
        res.status(200).json({
          message: "Login successful",
          email: email,
          userVerified: user.userVerified,
          userRole:user.role.name,
        });
      }
      else{
        res.status(200).json({
          message: "Login successful",
          email: email,
          userVerified: user.userVerified,
        });
      }
    }

  } catch (error) {
    console.error("Error verifying ID token:", error);
    res.status(400).json({ error: "Invalid ID Token" });
  }
});

// Forgot Password
router.post("/forgot-password", async (req, res) => {
  const { email } = req.body;

  if (!email) {
    return res.status(400).json({ error: "Email is required" });
  }

  try {
    // Request Firebase to generate password reset link
    await firebaseRequest("sendOobCode", {
      requestType: "PASSWORD_RESET",
      email,
    });

    res.status(200).json({ message: "Password reset link sent successfully. Check your email." });
  } catch (error) {
    console.error("Error sending password reset link:", error);
    res.status(400).json({ error: error.message });
  }
});
module.exports = router;
````

## File: BackEnd/routes/availabilityRoutes.js
````javascript
const express = require("express");
const verifyToken = require("../middleware/authMiddleware");
const { PrismaClient } = require("@prisma/client");


const prisma = new PrismaClient();
const availabilityRouter = express.Router();

// Convert Local Time to UTC Before Storing in DB
const convertToUTC = (dateString) => {
  return new Date(dateString).toISOString(); // Converts local datetime to UTC format
};

// // Convert UTC Time from DB to User's System Timezone Before Responding
// const convertToUserTimezone = (utcDate, userTimezone) => {
//   const date = new Date(utcDate);
//   if (isNaN(date.getTime())) return "Invalid Date"; // Prevents errors

//   return date.toISOString(); // Returns valid ISO 8601 format
// };


// ADD Availability (Store UTC in DB)
availabilityRouter.post("/add", verifyToken, async (req, res) => {
  try {
    const { startTime, endTime, status } = req.body;

    // Convert input time to UTC before storing
    const startTimeUTC = convertToUTC(startTime);
    const endTimeUTC = convertToUTC(endTime);

    const user = await prisma.user.findUnique({
      where: { email: req.user.email },
    });

    if (!user) {
      return res.status(404).json({ error: "User not found" });
    }

    const availability = await prisma.availability.create({
      data: {
        userId: user.id,
        startTime: startTimeUTC,
        endTime: endTimeUTC,
        status: status || "Available",
      },
    });

    res.json(availability);
  } catch (error) {
    console.error("Error creating availability:", error);
    res.status(500).json({ error: "Error creating availability" });
  }
});

// GET User Availability (Convert UTC to Local Time)
availabilityRouter.get("/byId", verifyToken, async (req, res) => {
  try {
    const user = await prisma.user.findUnique({
      where: { email: req.user.email },
    });

    if (!user) return res.status(404).json({ error: "User not found" });

    // Calculate UTC timestamp for 2 days ago
    const twoDaysAgo = new Date();
    twoDaysAgo.setDate(twoDaysAgo.getDate() - 2);

    // Fetch availability with UTC filter
    const availability = await prisma.availability.findMany({
      where: {
        userId: user.id,
        status: "Available",
        startTime: { gte: twoDaysAgo.toISOString() }, // Ensure startTime is >= 2 days ago (UTC)
      },
    });

    if (!availability.length) return res.status(200).json([]);

    // Convert UTC times to User's Timezone for display
    const userTimezone = Intl.DateTimeFormat().resolvedOptions().timeZone;

    const convertToUserTimezone = (date) =>
      new Date(date).toLocaleString("en-US", { timeZone: userTimezone });

    const formattedAvailability = availability.map((slot) => ({
      id: slot.id,
      startTime: convertToUserTimezone(slot.startTime),
      endTime: convertToUserTimezone(slot.endTime),
      status: slot.status,
    }));


    res.json(formattedAvailability);
  } catch (error) {
    console.error("Error fetching availability:", error);
    res.status(500).json({ error: "Error fetching availability" });
  }
});

// UPDATE Availability (Convert Local Time to UTC Before Updating)
availabilityRouter.put("/update/:id", verifyToken, async (req, res) => {
  try {
    const { id } = req.params;
    const { startTime, endTime, status } = req.body;

    const startTimeUTC = convertToUTC(startTime);
    const endTimeUTC = convertToUTC(endTime);

    const availability = await prisma.availability.update({
      where: { id: parseInt(id) },
      data: {
        startTime: startTimeUTC,
        endTime: endTimeUTC,
        status,
      },
    });

    res.json(availability);
  } catch (error) {
    console.error("Error updating availability:", error);
    res.status(500).json({ error: "Error updating availability" });
  }
});

// DELETE Availability (Added `verifyToken`)
availabilityRouter.delete("/delete/:id", verifyToken, async (req, res) => {
  try {
    const { id } = req.params;
    await prisma.availability.delete({
      where: { id: parseInt(id) },
    });
    res.json({ message: "Deleted successfully" });
  } catch (error) {
    console.error("Error deleting availability:", error);
    res.status(500).json({ error: "Error deleting availability" });
  }
});

//  GET Available Slots Based on Car or House Listing (Convert UTC to User's Timezone)


availabilityRouter.get("/express-interest", verifyToken, async (req, res) => {
  try {
    const { type, listingId } = req.query;

    if (!type || !listingId) {
      return res.status(400).json({ error: "Missing type or listingId" });
    }

    let listing, user;

    if (type === "car") {
      listing = await prisma.carListing.findUnique({
        where: { id: parseInt(listingId) },
        select: { dealershipId: true },
      });
      user = await prisma.user.findUnique({
        where: { id: listing?.dealershipId },
      });
    } else {
      listing = await prisma.houseListing.findUnique({
        where: { id: parseInt(listingId) },
        select: { landlordId: true },
      });
      user = await prisma.user.findUnique({
        where: { id: listing?.landlordId },
      });
    }

    if (!user) return res.status(404).json({ error: "Owner not found" });

    let availability = await prisma.availability.findMany({
      where: { userId: user.id, status: "Available" },
    });

    if (!availability.length) return res.status(200).json([]);

    // Get user timezone
    const userTimezone = Intl.DateTimeFormat().resolvedOptions().timeZone;

    // Get current time in user's timezone
    const currentTime = new Date().toLocaleString("en-US", { timeZone: userTimezone });

    const filteredAvailability = availability
      .map((slot) => ({
        id: slot.id,
        startTime: new Date(slot.startTime).toLocaleString("en-US", { timeZone: userTimezone }),
        endTime: new Date(slot.endTime).toLocaleString("en-US", { timeZone: userTimezone }),
        status: slot.status,
      }))
      .filter((slot) => new Date(slot.startTime) > new Date(currentTime));

    res.json(filteredAvailability);
  } catch (error) {
    console.error("Error fetching availability:", error);
    res.status(500).json({ error: "Error fetching availability" });
  }
});

availabilityRouter.get("/consultant-availability/:listingId", verifyToken, async (req, res) => {
  try {

    const { listingId } = req.params;
  
    // Fetch availability with UTC filter
    const availability = await prisma.availability.findMany({
      where: {
        userId: parseInt(listingId),
        status: "Available",
      },
    });

    if (!availability.length) return res.status(200).json([]);

    // Convert UTC times to User's Timezone for display
    const userTimezone = Intl.DateTimeFormat().resolvedOptions().timeZone;

    // Get current time in user's timezone
    const currentTime = new Date().toLocaleString("en-US", { timeZone: userTimezone });

    const filteredAvailability = availability
      .map((slot) => ({
        id: slot.id,
        startTime: new Date(slot.startTime).toLocaleString("en-US", { timeZone: userTimezone }),
        endTime: new Date(slot.endTime).toLocaleString("en-US", { timeZone: userTimezone }),
        status: slot.status,
      }))
      .filter((slot) => new Date(slot.startTime) > new Date(currentTime));


    res.json(filteredAvailability);
  } catch (error) {
    console.error("Error fetching availability:", error);
    res.status(500).json({ error: "Error fetching availability" });
  }
});



module.exports = availabilityRouter;
````

## File: BackEnd/routes/calendarAuthRoutes.js
````javascript
const express = require('express');
const { google } = require('googleapis');
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();
require('dotenv').config();

const router = express.Router();

// Google OAuth Configuration
const oauth2Client = new google.auth.OAuth2(
    process.env.GOOGLE_CLIENT_ID,
    process.env.GOOGLE_CLIENT_SECRET,
    process.env.GOOGLE_REDIRECT_URI,
);

// Step 1: Redirect User to Google Consent Page
router.get('/auth/google', (req, res) => {
    const authUrl = oauth2Client.generateAuthUrl({
        access_type: 'offline', // Needed for refresh token
        prompt: 'consent', // Forces re-consent if already signed in
        scope: [
            'https://www.googleapis.com/auth/calendar.events',
            'https://www.googleapis.com/auth/userinfo.email',
            'https://www.googleapis.com/auth/userinfo.profile',
        ]
    });

    res.redirect(authUrl);
});


// Step 2: Handle Google OAuth Callback
router.get('/auth/google/callback', async (req, res) => {
    try {
        const { code } = req.query;
        if (!code) return res.status(400).json({ error: 'Missing authorization code' });

        // Exchange authorization code for access token
        const { tokens } = await oauth2Client.getToken(code);
        if (!tokens.access_token) {
            return res.status(400).json({ error: 'Failed to obtain access token' });
        }

        // Set credentials before making API requests
        oauth2Client.setCredentials(tokens);

        // Use the access token to get user info
        const oauth2 = google.oauth2({ version: 'v2', auth: oauth2Client });
        const { data } = await oauth2.userinfo.get();

        if (!data.email) {
            return res.status(400).json({ error: 'Failed to retrieve user email' });
        }

        // Store refresh token in DB (only include fields that exist in Prisma)
        if (tokens.refresh_token) {
            await prisma.user.update({
                where: { email: data.email },
                data: { googleRefreshToken: tokens.refresh_token }
            });
        }

        res.json({ success: true, message: "Google Calendar connected successfully!", email: data.email });
    } catch (error) {
        console.error('OAuth Callback Error:', error);
        res.status(500).json({ error: 'OAuth authentication failed' });
    }
});

module.exports = router;
````

## File: BackEnd/routes/carListingRoutes.js
````javascript
const express = require('express');
const verifyToken = require('../middleware/authMiddleware');
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();
const multer = require('multer');

// Configure Multer for in-memory storage
const storage = multer.memoryStorage();
const upload = multer({ storage: storage });

const carListingRouter = express.Router();

carListingRouter.post('/add-car-listing', verifyToken, upload.array('images', 3), async (req, res) => {
    try {
        if (!req.body.model || !req.body.make || !req.body.price) {
            return res.status(400).json({ error: "Missing required fields: model, make, or price" });
        }

        const user = await prisma.user.findUnique({
            where: { email: req.user.email }
        });

        if (!user) {
            return res.status(404).json({ error: "User not found!" });
        }

        const { model, make, price, year, mileage, exteriorColor, interiorColor, transmission, vin, vehicleType, fuelType, noOfSeats, status } = req.body;
        const imageBuffers = req.files.map(file => ({ imageData: file.buffer }));

        const listing = await prisma.carListing.create({
            data: {
                model: model.trim(),
                make: make.trim(),
                price: parseFloat(price),
                year: parseInt(year),
                mileage: parseInt(mileage),
                exteriorColor: exteriorColor.trim(),
                interiorColor: interiorColor.trim(),
                transmission: transmission.trim(),
                vin: vin.trim(),
                vehicleType: vehicleType.trim(),
                fuelType: fuelType.trim(),
                noOfSeats: parseInt(noOfSeats),
                status: status.trim(),
                dealershipId: user.id,
                carImages: {
                    create: imageBuffers
                }
            },
            include: { carImages: true }
        });

        res.status(201).json({ message: "Car listing created successfully!", listing });
    } catch (error) {
        console.error("Error:", error);
        res.status(500).json({ error: "Internal Server Error" });
    }
});

carListingRouter.get('/all-car-listing', verifyToken, async (req, res) => {
    try {
        const carList = await prisma.carListing.findMany({
            include: { carImages: true }
        });

        if (!carList || carList.length === 0) {
            return res.status(404).json({ error: 'No car listings found' });
        }

        const formattedCarList = carList.map(car => ({
            ...car,
            carImages: car.carImages
                ? car.carImages.map(image => {
                    if (image.imageData && image.imageData instanceof Uint8Array) {
                        const base64String = `data:image/jpeg;base64,${Buffer.from(image.imageData).toString('base64')}`;
                        return {
                            id: image.id,
                            base64: base64String,
                        };
                    } else {
                        return {
                            id: image.id,
                            base64: null,
                        };
                    }
                })
                : [],
        }));

        res.status(200).json(formattedCarList);
    } catch (error) {
        console.error('Error fetching car listings:', error.message);
        res.status(500).json({ error: 'Failed to fetch car listings' });
    }
});

carListingRouter.get('/by-id-car-listing', verifyToken, async (req, res) => {
    try {
        const userWithListings = await prisma.user.findUnique({
            where: { email: req.user.email },
            include: {
                carListings: {
                    include: { carImages: true }
                }
            }
        });

        if (!userWithListings || userWithListings.carListings.length === 0) {
            return res.status(404).json({ error: 'No car listings found' });
        }

        const formattedCarList = userWithListings.carListings.map(car => ({
            ...car,
            carImages: car.carImages
                ? car.carImages.map(image => {
                    if (image.imageData && image.imageData instanceof Uint8Array) {
                        const base64String = `data:image/jpeg;base64,${Buffer.from(image.imageData).toString('base64')}`;
                        return {
                            id: image.id,
                            base64: base64String,
                        };
                    } else {
                        return {
                            id: image.id,
                            base64: null,
                        };
                    }
                })
                : [],
        }));

        res.status(200).json(formattedCarList);
    } catch (error) {
        console.error('Error fetching car listings:', error.message);
        res.status(500).json({ error: 'Failed to fetch car listings' });
    }
});

carListingRouter.get('/carlisting/:carListingId', verifyToken, async (req, res) => {
    try {
      const carListingId = parseInt(req.params.carListingId, 10);
  
      if (!carListingId) {
        return res.status(400).json({ error: 'houseListingId is required' });
      }
  
      // Ensure the listing exists before proceeding
      const carListing = await prisma.carListing.findUnique({
        where: { id: carListingId },
        select: { 
            id: true,
            make: true,
            model: true,
            price: true,
            year: true,
            mileage: true,
            exteriorColor: true,
            interiorColor: true,
            transmission: true,
            vin: true,
            vehicleType: true,
            noOfSeats: true,
            status: true,
            fuelType: true,
            createdAt:true,
            carImages: true, // Fetches all fields from the houseImages table
            dealership: { 
              select: { 
                fullName: true,
                phoneNo: true,
                email: true,
                carDealership: { 
                  select: { 
                    showroomLocations: true,
                    businessName: true,
                    financingOptions: true 
                  } 
                }
              } 
            }
          }
        });
  
      if (!carListing) {
        return res.status(404).json({ error: 'No house listings found' });
      }
  
      const formattedCarList = {
        ...carListing,
        carImages: carListing.carImages
          ? carListing.carImages.map(image => {
              // Convert Uint8Array to Base64 if valid
              if (image.imageData && image.imageData instanceof Uint8Array) {
                const base64String = `data:image/jpeg;base64,${Buffer.from(image.imageData).toString('base64')}`;
                return {
                  id: image.id,
                  base64: base64String,
                };
              } else {
                return {
                  id: image.id,
                  base64: null, // If imageData is invalid, return null
                };
              }
            })
          : [], // Ensure an empty array if no images
      };
  
      res.status(200).json(formattedCarList);
    } catch (error) {
      console.error('Error fetching car listings:', error.message);
      res.status(500).json({ error: 'Failed to fetch car listings' });
    }
  });

carListingRouter.delete('/delete-car-listing/:carListingId', verifyToken, async (req, res) => {
    try {
        const carListingId = parseInt(req.params.carListingId, 10);

        if (!carListingId) {
            return res.status(400).json({ error: 'carListingId is required' });
        }

        const carListing = await prisma.carListing.findUnique({
            where: { id: carListingId },
            include: { carImages: true }
        });

        if (!carListing) {
            return res.status(404).json({ error: 'Car listing not found' });
        }

        await prisma.carImage.deleteMany({
            where: { listingId: carListingId }
        });

        await prisma.carListing.delete({
            where: { id: carListingId }
        });

        res.status(200).json({ message: 'Car listing deleted successfully' });
    } catch (error) {
        console.error('Error deleting car listing:', error.message);
        res.status(500).json({ error: 'Failed to delete car listing' });
    }
});

carListingRouter.put('/update-car-listing/:id', verifyToken, upload.array('images', 3), async (req, res) => {
    try {
        const carId = parseInt(req.params.id);
        const { model, make, price, dealershipId,  year, mileage, exteriorColor, interiorColor, transmission, vin, vehicleType, fuelType, noOfSeats, status } = req.body;
        const imageBuffers = req.files.map(file => ({ imageData: file.buffer }));

        const updatedCar = await prisma.carListing.update({
            where: { id: carId },
            data: {
                model,
                make,
                price: parseFloat(price),
                dealershipId: dealershipId,
                year: parseInt(year, 10),
                mileage: parseInt(mileage, 10),
                exteriorColor: exteriorColor.trim(),
                interiorColor: interiorColor.trim(),
                transmission: transmission.trim(),
                vin: vin.trim(),
                vehicleType: vehicleType.trim(),
                fuelType: fuelType.trim(),
                noOfSeats: parseInt(noOfSeats),
                status: status.trim(),
                carImages: {
                    deleteMany: {},
                    create: imageBuffers
                }
            },
            include: { carImages: true }
        });

        res.status(200).json(updatedCar);
    } catch (error) {
        console.error('Error updating car listing:', error.message);
        res.status(500).json({ error: 'Failed to update car listing' });
    }
});

carListingRouter.delete('/delete-car-image/:id', verifyToken, async (req, res) => {
    try {
        const id = parseInt(req.params.id, 10);

        if (!id) {
            return res.status(400).json({ error: 'Image Id is required' });
        }

        await prisma.carImage.delete({
            where: { id: id }
        });

        res.status(200).json({ message: 'Car Image deleted successfully' });
    } catch (error) {
        console.error('Error deleting car image:', error.message);
        res.status(500).json({ error: 'Failed to delete car image' });
    }
});

// Add to FavouriteCar
carListingRouter.post('/add-to-favourites', verifyToken, async (req, res) => {
    const { listingId } = req.body;
  
    if (!listingId) {
      return res.status(400).json({ error: "listingId is required" });
    }
  
    try {
      const user = await prisma.user.findUnique({
        where: { email: req.user.email },
        include: { role: true }
      });
  
      if (!user) {
        return res.status(404).json({ error: "User not found" });
      }
  
      if (user.roleId !== 1) {
        return res.status(403).json({ error: "Only immigrants can add favourites" });
      }
  
      const favourite = await prisma.favouriteCar.create({
        data: {
          userId: user.id,
          listingId
        }
      });
  
      res.status(201).json({ message: "Car added to favourites", favourite });
    } catch (error) {
      if (error.code === 'P2002') {
        return res.status(400).json({ error: "Car already favourited" });
      }
      console.error("Add car to favourites error:", error);
      res.status(500).json({ error: "Failed to add to favourites" });
    }
  });

  // remove from favourite
  carListingRouter.delete('/remove-from-favourites/:listingId', verifyToken, async (req, res) => {
    const listingId = parseInt(req.params.listingId, 10);
  
    try {
      const user = await prisma.user.findUnique({
        where: { email: req.user.email }
      });
  
      if (!user) {
        return res.status(404).json({ error: 'User not found' });
      }
  
      await prisma.favouriteCar.delete({
        where: {
          userId_listingId: {
            userId: user.id,
            listingId
          }
        }
      });
  
      res.status(200).json({ message: 'Car removed from favourites' });
    } catch (error) {
      console.error("Remove favourite car error:", error);
      res.status(500).json({ error: 'Failed to remove car from favourites' });
    }
  });
  
  //All Favourite Cars
 carListingRouter.get('/favourites', verifyToken, async (req, res) => {
    try {
      const user = await prisma.user.findUnique({
        where: { email: req.user.email }
      });
  
      if (!user) {
        return res.status(404).json({ error: 'User not found' });
      }
  
      const favourites = await prisma.favouriteCar.findMany({
        where: { userId: user.id },
        include: {
          listing: {
            include: {
              carImages: true
            }
          }
        }
      });
  
      // Format image buffers
      const formatted = favourites.map(fav => {
        const listing = fav.listing;
  
        const formattedImages = listing.carImages.map(img => ({
          id: img.id,
          base64: img.imageData
            ? `data:image/jpeg;base64,${Buffer.from(img.imageData).toString('base64')}`
            : null
        }));
  
        return {
          ...listing,
          carImages: formattedImages
        };
      });
  
      res.status(200).json(formatted);
    } catch (error) {
      console.error("Fetch car favourites error:", error);
      res.status(500).json({ error: "Failed to fetch favourites" });
    }
  });
  
module.exports = carListingRouter;
````

## File: BackEnd/routes/consultantRoutes.js
````javascript
const express = require("express");
const verifyToken = require("../middleware/authMiddleware");
const { PrismaClient } = require("@prisma/client");


const prisma = new PrismaClient();
const consultantRouter = express.Router();



consultantRouter.get("/view-consultant", verifyToken, async (req, res) => {
    try {
      const user = await prisma.user.findUnique({
        where: { email: req.user.email },
      });
  
      if (!user) {
        return res.status(404).json({ error: "User not found" });
      }
  
      if (!user.countryOfOrigin) {
        return res.status(400).json({ error: "User's country of origin not set" });
      }
  
      const consultants = await prisma.immigrationConsultant.findMany({
        include: {
          user: true,
        },
      });
      if(user.alreadyInCanada){
        return res.status(200).json({ consultants: consultants });
      }
      const filteredConsultants = consultants.filter((consultant) => {
        const countries = consultant.countriesServed
          .split(",")
          .map((c) => c.trim().toLowerCase());
        return countries.includes(user.countryOfOrigin.toLowerCase());
      });
  
      return res.status(200).json({ consultants: filteredConsultants });
    } catch (error) {
      console.error("Error fetching consultants:", error);
      return res.status(500).json({ error: "Internal server error" });
    }
  });
  
  consultantRouter.get("/upcoming", verifyToken, async (req, res) => {
  try {
      const user = await prisma.user.findUnique({
        where: { email: req.user.email },
      });
  
      if (!user) {
        return res.status(404).json({ success: false, message: "User not found" });
      }
  
      const rawMeetings = await prisma.consultationBooking.findMany({
        where: {
          consultantId: user.id,
          startDate: {
            gte: new Date(Date.now() - 6 * 60 * 60 * 1000), // 6-hour buffer to catch borderline cases
          },
          status: "Confirmed",
        },
        orderBy: { startDate: "asc" },
        include: {
          user: {
            select: {
              fullName: true,
              email: true,
              phoneNo: true,
            },
          },
        },
      });
      
      const userTimezone = Intl.DateTimeFormat().resolvedOptions().timeZone;
      const nowInUserTZ = new Date().toLocaleString("en-US", { timeZone: userTimezone });
      const nowDate = new Date(nowInUserTZ);
  
      const convertToUserTimezone = (utcDate, userTimezone) => {
        const date = new Date(utcDate);
        if (isNaN(date.getTime())) return null;
        return new Date(date.toLocaleString("en-US", { timeZone: userTimezone }));
      };
  
      const upcoming = rawMeetings
        .map((meeting) => ({
          ...meeting,
          startDate: convertToUserTimezone(meeting.startDate, userTimezone),
        }))
        .filter((meeting) => meeting.startDate && meeting.startDate > nowDate)
        .sort((a, b) => a.startDate.getTime() - b.startDate.getTime())
        .slice(0, 3);
  
      return res.json({ success: true, meetings: upcoming });
    } catch (error) {
      console.error("Error fetching upcoming meetings:", error);
      return res.status(500).json({ success: false, message: "Server error" });
    }
  });
  

module.exports = consultantRouter;
````

## File: BackEnd/routes/dashboardRoutes.js
````javascript
const express = require("express");
const dashboardRouter = express.Router();
const verifyToken = require("../middleware/authMiddleware");//auth middleware 
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();

dashboardRouter.get("/profile", verifyToken, async(req, res) => {
  
  const user = await prisma.user.findUnique({
    where: {email: req.user.email},
    include: {role:true}
  
  });
  res.json(user);
});

  module.exports = dashboardRouter;
````

## File: BackEnd/routes/houseListingRoutes.js
````javascript
const express = require('express');
const verifyToken = require('../middleware/authMiddleware');
const { PrismaClient } = require('@prisma/client');
const prisma = new PrismaClient();
const multer = require('multer');

// Configure Multer for in-memory storage
const storage = multer.memoryStorage();
const upload = multer({ storage: storage });


const houseListingRouter = express.Router();

 // Change this to match the field name in Postman
  
  houseListingRouter.post('/add-house-listing', verifyToken, upload.array('images', 3), async (req, res) => {
    try {

        // Validate request body
        if (!req.body.title || !req.body.price || !req.body.location) {
            return res.status(400).json({ error: "Missing required fields: title, price, or location" });
        }

        const user = await prisma.user.findUnique({
            where: { email: req.user.email }
        });

        if (!user) {
            return res.status(404).json({ error: "User not found!" });
        }

        const { title, description, price, location, openhouse, bedrooms, bathrooms, sqft } = req.body;
         // Convert uploaded images to Buffer
        const imageBuffers = req.files.map(file => ({
          imageData: file.buffer // Save image as Buffer (BLOB)
        }));;

        // Create House Listing
        const listing = await prisma.houseListing.create({
            data: {
                title: title.trim(),
                description: description ? description.trim() : null,
                price: parseFloat(price) || 0, // Ensure it's a valid number
                location: location.trim(),
                landlordId: user.id,
                bedrooms: parseInt(bedrooms),
                bathrooms: parseInt(bathrooms),
                squareFeet: parseInt(sqft),
                openhouse : JSON.parse(openhouse) ? JSON.parse(openhouse) : false,
                startdate : JSON.parse(openhouse) ? new Date(req.body.startDate) : null,
                endDate : JSON.parse(openhouse) ? new Date(req.body.endDate) : null,
                startTime: JSON.parse(openhouse) ? req.body.startTime : null,
                endTime: JSON.parse(openhouse) ? req.body.endTime : null,
                houseImages: {
                  create: imageBuffers // Insert new images as BLOB
              }
            },
            include: { houseImages: true } 
        });

  

        res.status(201).json({ message: "Listing created successfully!", listing });
    } catch (error) {
        console.error(" Error:", error);
        res.status(500).json({ error: "Internal Server Error" });
    }
});

houseListingRouter.get('/download/:documentId', verifyToken, async (req, res) => {
    try {
      // Get the documentId from the request params
      const documentId = parseInt(req.params.documentId, 10);
  
      // Retrieve the image from the database (assuming you store the image as a buffer in `houseImage`)
      const document = await prisma.houseImage.findUnique({
        where: { id: documentId }
      });
  
      if (!document) {
        return res.status(404).json({ error: 'Image not found' });
      }
  
      // Set appropriate headers for the response based on file type
      const mimeType = 'image/jpeg';  // You can dynamically set this based on the file type if needed
  
      res.setHeader('Content-Type', mimeType);  // Set the correct MIME type for the image
      res.setHeader('Content-Disposition', `attachment; filename="image_${documentId}.jpg"`);  // Change file name as needed
  
      // Send the file buffer directly to the response
      res.end(document.imageData);  // This sends the image data as a response to the client
    } catch (error) {
      console.error('Error:', error.message);
      res.status(500).json({ error: 'Failed to download image' });
    }
  });

  houseListingRouter.get('/all-house-listing', verifyToken, async (req, res) => {
    try {
      const houseList = await prisma.houseListing.findMany({
        include: {
          houseImages: true, // Ensure images are included
        },
      });
  
      if (!houseList || houseList.length === 0) {
        return res.status(404).json({ error: 'No house listings found' });
      }
  
      const formattedHouseList = houseList.map(house => ({
        ...house,
        houseImages: house.houseImages
          ? house.houseImages.map(image => {
              // Convert Uint8Array to Base64
              if (image.imageData && image.imageData instanceof Uint8Array) {
                const base64String = `data:image/jpeg;base64,${Buffer.from(image.imageData).toString('base64')}`;
                return {
                  id: image.id,
                  base64: base64String,
                };
              } else {
                return {
                  id: image.id,
                  base64: null, // If imageData is invalid, return null
                };
              }
            })
          : [],
      }));
  
      res.status(200).json(formattedHouseList);
    } catch (error) {
      console.error('Error fetching house listings:', error.message);
      res.status(500).json({ error: 'Failed to fetch house listings' });
    }
  });

  houseListingRouter.get('/by-id-house-listing', verifyToken, async (req, res) => {
    try {

 
      const userWithListings = await prisma.user.findUnique({
        where: { email: req.user.email },
        include: {
          houseListings: {
            include: {
              houseImages: true, // Fetch images for each house listing
            },
          },
        },
      });

  
      if (!userWithListings || userWithListings.length === 0) {
        return res.status(404).json({ error: 'No house listings found' });
      }
  
      const formattedHouseList = userWithListings.houseListings.map(house => ({
        ...house,
        houseImages: house.houseImages
          ? house.houseImages.map(image => {
              // Convert Uint8Array to Base64
              if (image.imageData && image.imageData instanceof Uint8Array) {
                const base64String = `data:image/jpeg;base64,${Buffer.from(image.imageData).toString('base64')}`;
                return {
                  id: image.id,
                  base64: base64String,
                };
              } else {
                return {
                  id: image.id,
                  base64: null, // If imageData is invalid, return null
                };
              }
            })
          : [],
      }));
  
      res.status(200).json(formattedHouseList);
    } catch (error) {
      console.error('Error fetching house listings:', error.message);
      res.status(500).json({ error: 'Failed to fetch house listings' });
    }
  });

  houseListingRouter.get('/houselisting/:houseListingId', verifyToken, async (req, res) => {
    try {
      const houseListingId = parseInt(req.params.houseListingId, 10);
  
      if (!houseListingId) {
        return res.status(400).json({ error: 'houseListingId is required' });
      }
  
      // Ensure the listing exists before proceeding
      const houseListing = await prisma.houseListing.findUnique({
        where: { id: houseListingId },
        select: { 
          id: true,
          title: true,
          description: true,
          price: true,
          location:true,
          bedrooms: true,
          bathrooms: true,
          squareFeet:true,
          openhouse:true,
          startdate: true,
          endDate: true,
          startTime: true,
          endTime: true,
          createdAt:true,
          houseImages: true, 
          landlord: { 
            select: { 
              fullName: true,
              phoneNo: true,
              email: true,
              realtor: { 
                select: { 
                  businessName: true,
                  businessAddress: true,
                  portfolioWebsite: true 
                } 
              }
            } 
          }
        }
      });
       
  
      if (!houseListing) {
        return res.status(404).json({ error: 'No house listings found' });
      }
  
      const formattedHouseList = {
        ...houseListing,
        houseImages: houseListing.houseImages
          ? houseListing.houseImages.map(image => {
              // Convert Uint8Array to Base64 if valid
              if (image.imageData && image.imageData instanceof Uint8Array) {
                const base64String = `data:image/jpeg;base64,${Buffer.from(image.imageData).toString('base64')}`;
                return {
                  id: image.id,
                  base64: base64String,
                };
              } else {
                return {
                  id: image.id,
                  base64: null, // If imageData is invalid, return null
                };
              }
            })
          : [], // Ensure an empty array if no images
      };
  
      res.status(200).json(formattedHouseList);
    } catch (error) {
      console.error('Error fetching house listings:', error.message);
      res.status(500).json({ error: 'Failed to fetch house listings' });
    }
  });
  

  houseListingRouter.delete('/delete-house-listing/:houseListingId', verifyToken, async (req, res) => {
    try {
      const houseListingId = parseInt(req.params.houseListingId, 10)
  
      if (!houseListingId) {
        return res.status(400).json({ error: 'houseListingId is required' });
      }
  
      // Ensure the listing exists before deleting
      const houseListing = await prisma.houseListing.findUnique({
        where: { id: houseListingId },
        include: { houseImages: true }, // To check if images exist
      });
  
      if (!houseListing) {
        return res.status(404).json({ error: 'House listing not found' });
      }
  
      // Delete house images first (only needed if cascade delete is not enabled in Prisma schema)
      await prisma.houseImage.deleteMany({
        where: { listingId: houseListingId },
      });
  
      // Delete the house listing
      await prisma.houseListing.delete({
        where: { id: houseListingId },
      });
  
      res.status(200).json({ message: 'House listing deleted successfully' });
    } catch (error) {
      console.error('Error deleting house listing:', error.message);
      res.status(500).json({ error: 'Failed to delete house listing' });
    }
  });
  
  
houseListingRouter.put('/update-house-listing/:id', verifyToken, upload.array('images', 3), async (req, res) => {
  try {
    const houseId = parseInt(req.params.id);
    const { title, description, price, location, landlordId, openhouse, bedrooms, bathrooms, sqft} = req.body;
    
    // Convert uploaded images to Buffer
    const imageBuffers = req.files.map(file => ({
        imageData: file.buffer // Save image as Buffer (BLOB)
    }));

    // Update house listing and images
    const updatedHouse = await prisma.houseListing.update({
        where: { id: houseId },
        data: {
            title,
            description,
            price: parseFloat(price),
            location,
            landlordId: landlordId,
            bedrooms: parseInt(bedrooms),
            bathrooms: parseInt(bathrooms),
            squareFeet: parseInt(sqft),
            openhouse : JSON.parse(openhouse) ? JSON.parse(openhouse) : false,
            startdate : JSON.parse(openhouse) ? new Date(req.body.startDate) : null,
            endDate : JSON.parse(openhouse) ? new Date(req.body.endDate) : null,
            startTime: JSON.parse(openhouse) ? req.body.startTime : null,
            endTime: JSON.parse(openhouse) ? req.body.endTime : null,
            houseImages: {
                deleteMany: {}, // Delete old images (optional)
                create: imageBuffers // Insert new images as BLOB
            }
        },
        include: { houseImages: true } // Return updated images
    });

    res.status(200).json(updatedHouse);
} catch (error) {
    console.error('Error updating house listing:', error.message);
    res.status(500).json({ error: 'Failed to update house listing' });
}
});

houseListingRouter.put('/openhouse/:id', verifyToken, async (req, res) => {
  try {
    const houseId = parseInt(req.params.id);
 

    // Update house listing and images
    const updatedHouse = await prisma.houseListing.update({
        where: { id: houseId },
        data: {
           
            openhouse : JSON.parse(req.body.openhouse) ? JSON.parse(req.body.openhouse) : false,
            startdate : JSON.parse(req.body.openhouse) ? new Date(req.body.startDate) : null,
            endDate : JSON.parse(req.body.openhouse) ? new Date(req.body.endDate) : null,
            startTime: JSON.parse(req.body.openhouse) ? req.body.startTime : null,
            endTime: JSON.parse(req.body.openhouse) ? req.body.endTime : null,
           
        } 
    });

    res.status(200).json(updatedHouse);
} catch (error) {
    console.error('Error updating house listing:', error.message);
    res.status(500).json({ error: 'Failed to update house listing' });
}
});


houseListingRouter.delete('/delete-house-image/:id', verifyToken, async (req, res) => {
  try {
    const id = parseInt(req.params.id, 10)

    if (!id) {
      return res.status(400).json({ error: 'Image Id is required' });
    }

    // Delete house image
    await prisma.houseImage.delete({
      where: { id: id },
    });

    res.status(200).json({ message: 'House Image deleted successfully' });
  } catch (error) {
    console.error('Error deleting house listing:', error.message);
    res.status(500).json({ error: 'Failed to delete house listing' });
  }
});
  

// Add to FavouriteHouse

houseListingRouter.post('/add-to-favourites', verifyToken, async (req, res) => {
  const { listingId } = req.body;
  // const firebaseUid = req.user.user_id;

  if (!listingId) {
    return res.status(400).json({ error: 'listingId is required' });
  }

  try {
    const user = await prisma.user.findUnique({
      where: {email:req.user.email },
      include: { role: true } // to get roleId or role name
    });

    if (!user) {
      return res.status(404).json({ error: 'User not found' });
    }

    // Check if user is immigrant
    if (user.roleId !== 1) {
      return res.status(403).json({ error: 'Only immigrants can add favourites' });
    }

    const favourite = await prisma.favouriteHouse.create({
      data: {
        userId: user.id,
        listingId
      }
    });

    res.status(201).json({ message: 'House added to favourites', favourite });

  } catch (error) {
    console.error("Add house to favourites error:", error);
    res.status(500).json({ error: 'Failed to add to favourites' });
  }
});

//remove from FavouriteHouse
houseListingRouter.delete('/remove-from-favourites/:listingId', verifyToken, async (req, res) => {
  const listingId = parseInt(req.params.listingId, 10);
  // const firebaseUid = req.user.user_id;
  console.log('Decoded Firebase UID:', req.user.user_id);
  try {
    const user = await prisma.user.findUnique({
      where: { email:req.user.email }
    });

    if (!user) {
      return res.status(404).json({ error: 'User not found' });
    }

    await prisma.favouriteHouse.delete({
      where: {
        userId_listingId: {
          userId: user.id,      
          listingId
        }
      }
    });

    res.status(200).json({ message: 'House removed from favourites' });

  } catch (error) {
    console.error('Remove favourite error:', error);
    res.status(500).json({ error: 'Failed to remove house from favourites' });
  }
});

//all favourites
houseListingRouter.get('/favourites', verifyToken, async (req, res) => {
  try {
    const user = await prisma.user.findUnique({
      where: { email: req.user.email }
    });

    if (!user) {
      return res.status(404).json({ error: 'User not found' });
    }

    const favourites = await prisma.favouriteHouse.findMany({
      where: {
        userId: user.id,
      },
      include: {
        listing: {
          include: {
            houseImages: true
          }
        }
      }
    });

    // Extract and format listing data including images
    const listings = favourites.map(fav => {
      const listing = fav.listing;
      const formattedImages = listing.houseImages.map(image => ({
        id: image.id,
        base64: image.imageData
          ? `data:image/jpeg;base64,${Buffer.from(image.imageData).toString('base64')}`
          : null,
      }));

      return {
        ...listing,
        houseImages: formattedImages
      };
    });

    res.status(200).json(listings);
  } catch (error) {
    console.error('Fetch house favourites error:', error);
    res.status(500).json({ error: 'Failed to fetch favourite houses' });
  }
});

module.exports = houseListingRouter;
````

## File: BackEnd/routes/onboardingRoutes.js
````javascript
const express = require('express');
const verifyToken = require('../middleware/authMiddleware');
const roleBasedData = require('../middleware/roleBasedDataMiddleware');
const uploadDocuments = require('../middleware/uploadFileMiddleware'); // Import file upload middleware
const { PrismaClient } = require('@prisma/client');

const prisma = new PrismaClient();
const onboardingRouter = express.Router();


onboardingRouter.post('/information', verifyToken,uploadDocuments, roleBasedData, async (req, res) => {
    try {
        // Validate uploaded documents based on role
        if (req.body.rolename === 'Immigrant' && !req.files['govId']) {
            return res.status(400).json({ error: 'Government ID is required for Immigrants.' });
        }

        if (req.body.rolename !== 'Immigrant' && (!req.files['govId'] || !req.files['businessDoc'] || !req.files['licenseCert'])) {
            return res.status(400).json({ error: 'All documents (Gov ID, Business Doc, License Cert) are required for this role.' });
        }

        // Start transaction
        const newUser = await prisma.$transaction(async (tx) => {
            // Create user
            const user = await tx.user.create({
                data: {
                    fullName: req.body.fullName,
                    DOB: new Date(req.body.DOB),
                    phoneNo: req.body.phoneNo,
                    email: req.user.email,
                    firebaseUid: req.user.uid,
                    alreadyInCanada: req.body.alreadyInCanada === "true" ? true : false,
                    countryOfOrigin: req.body.countryOfOrigin,
                    currentLocation: req.body.workSchoolLocation,
                    statusInCanada: req.body.statusInCanada || null,
                    roleId: req.body.roleId,
                    backgroundVerification: JSON.parse(req.body.backgroundVerification),
                    termsConditionCheck: JSON.parse(req.body.termsConditionCheck),

                    realtor: req.body.realtorData ? { create: req.body.realtorData } : undefined,
                    carDealership: req.body.carDealershipData ? { create: req.body.carDealershipData } : undefined,
                    immigrationConsultant: req.body.immigrationConsultantData
                        ? { create: req.body.immigrationConsultantData }
                        : undefined
                }
            });

            // Store uploaded files in the database
            const documents = [];

            if (req.files['govId']) {
                documents.push({
                    userId: user.id,
                    documentType: 'Government-Issued ID',
                    fileData: req.files['govId'][0].buffer
                });
            }

            if (req.body.roleName !== 'Immigrant') {
                if (req.files['businessDoc']) {
                    documents.push({
                        userId: user.id,
                        documentType: 'Business Verification Document',
                        fileData: req.files['businessDoc'][0].buffer
                    });
                }

                if (req.files['licenseCert']) {
                    documents.push({
                        userId: user.id,
                        documentType: 'License/Accreditation Certificate',
                        fileData: req.files['licenseCert'][0].buffer
                    });
                }
            }

            if (documents.length > 0) {
                await tx.userDocument.createMany({ data: documents });
            }

            return user;
        });

        res.status(201).json({ message: 'User and documents uploaded successfully', user: newUser });
    } catch (error) {
        console.error('Error:', error.message);
        res.status(500).json({ error: 'Failed to create user and upload documents' });
    }
});


onboardingRouter.get('/download/:documentId', verifyToken, async (req, res) => {
  try {
    // Get the documentId from the request params
    const documentId = parseInt(req.params.documentId, 10);

    // Retrieve the document from the database
    const document = await prisma.userDocument.findUnique({
      where: { id: documentId }
    });

    if (!document) {
      return res.status(404).json({ error: 'Document not found' });
    }

    // Set appropriate headers for the response
    // Assuming the document is a PDF, change this for other file types (e.g., image/png, image/jpeg)
    res.setHeader('Content-Type', 'application/pdf');  // Set the correct MIME type for the document
    res.setHeader('Content-Disposition', `attachment; filename="${document.documentType}.pdf"`);  // Change the file name as needed

    // Send the file buffer directly to the response
    res.end(document.fileData);  // This sends the actual file content as a response to the client
  } catch (error) {
    console.error('Error:', error.message);
    res.status(500).json({ error: 'Failed to download document' });
  }
});


module.exports = onboardingRouter;
````

## File: BackEnd/testIframe.html
````html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PDF Viewer</title>
</head>
<body>

    <h2>View PDF Document</h2>

    <iframe 
        id="pdfViewer"
        width="100%" 
        height="600px"
        style="border: none;">
    </iframe>

    <script>
        // Replace this with your actual JWT token
        const token = "eyJhbGciOiJSUzI1NiIsImtpZCI6ImJjNDAxN2U3MGE4MWM5NTMxY2YxYjY4MjY4M2Q5OThlNGY1NTg5MTkiLCJ0eXAiOiJKV1QifQ.eyJpc3MiOiJodHRwczovL3NlY3VyZXRva2VuLmdvb2dsZS5jb20vaW1taWdyYXRleC1haS1odW1iZXIiLCJhdWQiOiJpbW1pZ3JhdGV4LWFpLWh1bWJlciIsImF1dGhfdGltZSI6MTc0MTY0MDg3NSwidXNlcl9pZCI6ImhVcTJvM3RObnZOdGNVck1RWkM3VW8xd2M1TDIiLCJzdWIiOiJoVXEybzN0Tm52TnRjVXJNUVpDN1VvMXdjNUwyIiwiaWF0IjoxNzQxNjQwODc1LCJleHAiOjE3NDE2NDQ0NzUsImVtYWlsIjoic2FtY2hhdmFueGl2OUBnbWFpbC5jb20iLCJlbWFpbF92ZXJpZmllZCI6dHJ1ZSwiZmlyZWJhc2UiOnsiaWRlbnRpdGllcyI6eyJlbWFpbCI6WyJzYW1jaGF2YW54aXY5QGdtYWlsLmNvbSJdfSwic2lnbl9pbl9wcm92aWRlciI6InBhc3N3b3JkIn19.tf0evWKafSzZp0-qvYQiNoeuSDOSsfsim8LVe1yHRqaq5g2tRMi2j1uAhRGn-C1QmuK16Kp7-8sITrYFu__AOrCxOjocf7dBVgF2_Jt--Xsbl4E48_VBSkVQ_mhuDyujZVMtJ5lyfzWftmHsBejwqY-Nu_Fcc5a4jHhZa3o6R1wqLMmygq9UKebbtciNjahRAWFZ2TnB0S28j-6p5tVbGd_vW0fHB2ITmvtnqihEJw06msinXuxBHcsqET8gkSENEE2y3HiwC_DegG91An2wnLKrQrULa0empxHqBTsccOQsvEz_R24GPzMi2Rd-2qLqxwSOqYxJbx8GA9f7dZcCPQ"; // This token should be securely fetched or stored
        const documentId = 61; // Replace with actual document ID

        // Fetch the PDF document with the Authorization header
        fetch(`http://localhost:5500/api/admin/user-list/user-document/${documentId}`, {
            method: 'GET',
            headers: {
                'Authorization': `Bearer ${token}`,
            },
        })
        .then(response => response.blob()) // Get the response as a Blob
        .then(blob => {
            const url = URL.createObjectURL(blob); // Create an object URL for the Blob
            document.getElementById("pdfViewer").src = url; // Set the iframe source
        })
        .catch(error => {
            console.error("Error loading the document:", error);
        });
    </script>

</body>
</html>
````

## File: Frontend/.git/config
````
[core]
	repositoryformatversion = 0
	filemode = false
	bare = false
	logallrefupdates = true
	symlinks = false
	ignorecase = true
[remote "origin"]
	url = https://github.com/rajatsachdeva31/ImmiGrowAI-Frontend.git
	fetch = +refs/heads/*:refs/remotes/origin/*
[branch "main"]
	remote = origin
	merge = refs/heads/main
	vscode-merge-base = origin/main
````

## File: Frontend/.git/description
````
Unnamed repository; edit this file 'description' to name the repository.
````

## File: Frontend/.git/FETCH_HEAD
````
3324131b0dd5a90a5485178d1251e140d9ae4aa6		branch 'main' of https://github.com/rajatsachdeva31/ImmiGrowAI-Frontend
````

## File: Frontend/.git/HEAD
````
ref: refs/heads/main
````

## File: Frontend/.git/hooks/applypatch-msg.sample
````
#!/bin/sh
#
# An example hook script to check the commit log message taken by
# applypatch from an e-mail message.
#
# The hook should exit with non-zero status after issuing an
# appropriate message if it wants to stop the commit.  The hook is
# allowed to edit the commit message file.
#
# To enable this hook, rename this file to "applypatch-msg".

. git-sh-setup
commitmsg="$(git rev-parse --git-path hooks/commit-msg)"
test -x "$commitmsg" && exec "$commitmsg" ${1+"$@"}
:
````

## File: Frontend/.git/hooks/commit-msg.sample
````
#!/bin/sh
#
# An example hook script to check the commit log message.
# Called by "git commit" with one argument, the name of the file
# that has the commit message.  The hook should exit with non-zero
# status after issuing an appropriate message if it wants to stop the
# commit.  The hook is allowed to edit the commit message file.
#
# To enable this hook, rename this file to "commit-msg".

# Uncomment the below to add a Signed-off-by line to the message.
# Doing this in a hook is a bad idea in general, but the prepare-commit-msg
# hook is more suited to it.
#
# SOB=$(git var GIT_AUTHOR_IDENT | sed -n 's/^\(.*>\).*$/Signed-off-by: \1/p')
# grep -qs "^$SOB" "$1" || echo "$SOB" >> "$1"

# This example catches duplicate Signed-off-by lines.

test "" = "$(grep '^Signed-off-by: ' "$1" |
	 sort | uniq -c | sed -e '/^[ 	]*1[ 	]/d')" || {
	echo >&2 Duplicate Signed-off-by lines.
	exit 1
}
````

## File: Frontend/.git/hooks/fsmonitor-watchman.sample
````
#!/usr/bin/perl

use strict;
use warnings;
use IPC::Open2;

# An example hook script to integrate Watchman
# (https://facebook.github.io/watchman/) with git to speed up detecting
# new and modified files.
#
# The hook is passed a version (currently 2) and last update token
# formatted as a string and outputs to stdout a new update token and
# all files that have been modified since the update token. Paths must
# be relative to the root of the working tree and separated by a single NUL.
#
# To enable this hook, rename this file to "query-watchman" and set
# 'git config core.fsmonitor .git/hooks/query-watchman'
#
my ($version, $last_update_token) = @ARGV;

# Uncomment for debugging
# print STDERR "$0 $version $last_update_token\n";

# Check the hook interface version
if ($version ne 2) {
	die "Unsupported query-fsmonitor hook version '$version'.\n" .
	    "Falling back to scanning...\n";
}

my $git_work_tree = get_working_dir();

my $retry = 1;

my $json_pkg;
eval {
	require JSON::XS;
	$json_pkg = "JSON::XS";
	1;
} or do {
	require JSON::PP;
	$json_pkg = "JSON::PP";
};

launch_watchman();

sub launch_watchman {
	my $o = watchman_query();
	if (is_work_tree_watched($o)) {
		output_result($o->{clock}, @{$o->{files}});
	}
}

sub output_result {
	my ($clockid, @files) = @_;

	# Uncomment for debugging watchman output
	# open (my $fh, ">", ".git/watchman-output.out");
	# binmode $fh, ":utf8";
	# print $fh "$clockid\n@files\n";
	# close $fh;

	binmode STDOUT, ":utf8";
	print $clockid;
	print "\0";
	local $, = "\0";
	print @files;
}

sub watchman_clock {
	my $response = qx/watchman clock "$git_work_tree"/;
	die "Failed to get clock id on '$git_work_tree'.\n" .
		"Falling back to scanning...\n" if $? != 0;

	return $json_pkg->new->utf8->decode($response);
}

sub watchman_query {
	my $pid = open2(\*CHLD_OUT, \*CHLD_IN, 'watchman -j --no-pretty')
	or die "open2() failed: $!\n" .
	"Falling back to scanning...\n";

	# In the query expression below we're asking for names of files that
	# changed since $last_update_token but not from the .git folder.
	#
	# To accomplish this, we're using the "since" generator to use the
	# recency index to select candidate nodes and "fields" to limit the
	# output to file names only. Then we're using the "expression" term to
	# further constrain the results.
	my $last_update_line = "";
	if (substr($last_update_token, 0, 1) eq "c") {
		$last_update_token = "\"$last_update_token\"";
		$last_update_line = qq[\n"since": $last_update_token,];
	}
	my $query = <<"	END";
		["query", "$git_work_tree", {$last_update_line
			"fields": ["name"],
			"expression": ["not", ["dirname", ".git"]]
		}]
	END

	# Uncomment for debugging the watchman query
	# open (my $fh, ">", ".git/watchman-query.json");
	# print $fh $query;
	# close $fh;

	print CHLD_IN $query;
	close CHLD_IN;
	my $response = do {local $/; <CHLD_OUT>};

	# Uncomment for debugging the watch response
	# open ($fh, ">", ".git/watchman-response.json");
	# print $fh $response;
	# close $fh;

	die "Watchman: command returned no output.\n" .
	"Falling back to scanning...\n" if $response eq "";
	die "Watchman: command returned invalid output: $response\n" .
	"Falling back to scanning...\n" unless $response =~ /^\{/;

	return $json_pkg->new->utf8->decode($response);
}

sub is_work_tree_watched {
	my ($output) = @_;
	my $error = $output->{error};
	if ($retry > 0 and $error and $error =~ m/unable to resolve root .* directory (.*) is not watched/) {
		$retry--;
		my $response = qx/watchman watch "$git_work_tree"/;
		die "Failed to make watchman watch '$git_work_tree'.\n" .
		    "Falling back to scanning...\n" if $? != 0;
		$output = $json_pkg->new->utf8->decode($response);
		$error = $output->{error};
		die "Watchman: $error.\n" .
		"Falling back to scanning...\n" if $error;

		# Uncomment for debugging watchman output
		# open (my $fh, ">", ".git/watchman-output.out");
		# close $fh;

		# Watchman will always return all files on the first query so
		# return the fast "everything is dirty" flag to git and do the
		# Watchman query just to get it over with now so we won't pay
		# the cost in git to look up each individual file.
		my $o = watchman_clock();
		$error = $output->{error};

		die "Watchman: $error.\n" .
		"Falling back to scanning...\n" if $error;

		output_result($o->{clock}, ("/"));
		$last_update_token = $o->{clock};

		eval { launch_watchman() };
		return 0;
	}

	die "Watchman: $error.\n" .
	"Falling back to scanning...\n" if $error;

	return 1;
}

sub get_working_dir {
	my $working_dir;
	if ($^O =~ 'msys' || $^O =~ 'cygwin') {
		$working_dir = Win32::GetCwd();
		$working_dir =~ tr/\\/\//;
	} else {
		require Cwd;
		$working_dir = Cwd::cwd();
	}

	return $working_dir;
}
````

## File: Frontend/.git/hooks/post-update.sample
````
#!/bin/sh
#
# An example hook script to prepare a packed repository for use over
# dumb transports.
#
# To enable this hook, rename this file to "post-update".

exec git update-server-info
````

## File: Frontend/.git/hooks/pre-applypatch.sample
````
#!/bin/sh
#
# An example hook script to verify what is about to be committed
# by applypatch from an e-mail message.
#
# The hook should exit with non-zero status after issuing an
# appropriate message if it wants to stop the commit.
#
# To enable this hook, rename this file to "pre-applypatch".

. git-sh-setup
precommit="$(git rev-parse --git-path hooks/pre-commit)"
test -x "$precommit" && exec "$precommit" ${1+"$@"}
:
````

## File: Frontend/.git/hooks/pre-commit.sample
````
#!/bin/sh
#
# An example hook script to verify what is about to be committed.
# Called by "git commit" with no arguments.  The hook should
# exit with non-zero status after issuing an appropriate message if
# it wants to stop the commit.
#
# To enable this hook, rename this file to "pre-commit".

if git rev-parse --verify HEAD >/dev/null 2>&1
then
	against=HEAD
else
	# Initial commit: diff against an empty tree object
	against=$(git hash-object -t tree /dev/null)
fi

# If you want to allow non-ASCII filenames set this variable to true.
allownonascii=$(git config --type=bool hooks.allownonascii)

# Redirect output to stderr.
exec 1>&2

# Cross platform projects tend to avoid non-ASCII filenames; prevent
# them from being added to the repository. We exploit the fact that the
# printable range starts at the space character and ends with tilde.
if [ "$allownonascii" != "true" ] &&
	# Note that the use of brackets around a tr range is ok here, (it's
	# even required, for portability to Solaris 10's /usr/bin/tr), since
	# the square bracket bytes happen to fall in the designated range.
	test $(git diff-index --cached --name-only --diff-filter=A -z $against |
	  LC_ALL=C tr -d '[ -~]\0' | wc -c) != 0
then
	cat <<\EOF
Error: Attempt to add a non-ASCII file name.

This can cause problems if you want to work with people on other platforms.

To be portable it is advisable to rename the file.

If you know what you are doing you can disable this check using:

  git config hooks.allownonascii true
EOF
	exit 1
fi

# If there are whitespace errors, print the offending file names and fail.
exec git diff-index --check --cached $against --
````

## File: Frontend/.git/hooks/pre-merge-commit.sample
````
#!/bin/sh
#
# An example hook script to verify what is about to be committed.
# Called by "git merge" with no arguments.  The hook should
# exit with non-zero status after issuing an appropriate message to
# stderr if it wants to stop the merge commit.
#
# To enable this hook, rename this file to "pre-merge-commit".

. git-sh-setup
test -x "$GIT_DIR/hooks/pre-commit" &&
        exec "$GIT_DIR/hooks/pre-commit"
:
````

## File: Frontend/.git/hooks/pre-push.sample
````
#!/bin/sh

# An example hook script to verify what is about to be pushed.  Called by "git
# push" after it has checked the remote status, but before anything has been
# pushed.  If this script exits with a non-zero status nothing will be pushed.
#
# This hook is called with the following parameters:
#
# $1 -- Name of the remote to which the push is being done
# $2 -- URL to which the push is being done
#
# If pushing without using a named remote those arguments will be equal.
#
# Information about the commits which are being pushed is supplied as lines to
# the standard input in the form:
#
#   <local ref> <local oid> <remote ref> <remote oid>
#
# This sample shows how to prevent push of commits where the log message starts
# with "WIP" (work in progress).

remote="$1"
url="$2"

zero=$(git hash-object --stdin </dev/null | tr '[0-9a-f]' '0')

while read local_ref local_oid remote_ref remote_oid
do
	if test "$local_oid" = "$zero"
	then
		# Handle delete
		:
	else
		if test "$remote_oid" = "$zero"
		then
			# New branch, examine all commits
			range="$local_oid"
		else
			# Update to existing branch, examine new commits
			range="$remote_oid..$local_oid"
		fi

		# Check for WIP commit
		commit=$(git rev-list -n 1 --grep '^WIP' "$range")
		if test -n "$commit"
		then
			echo >&2 "Found WIP commit in $local_ref, not pushing"
			exit 1
		fi
	fi
done

exit 0
````

## File: Frontend/.git/hooks/pre-rebase.sample
````
#!/bin/sh
#
# Copyright (c) 2006, 2008 Junio C Hamano
#
# The "pre-rebase" hook is run just before "git rebase" starts doing
# its job, and can prevent the command from running by exiting with
# non-zero status.
#
# The hook is called with the following parameters:
#
# $1 -- the upstream the series was forked from.
# $2 -- the branch being rebased (or empty when rebasing the current branch).
#
# This sample shows how to prevent topic branches that are already
# merged to 'next' branch from getting rebased, because allowing it
# would result in rebasing already published history.

publish=next
basebranch="$1"
if test "$#" = 2
then
	topic="refs/heads/$2"
else
	topic=`git symbolic-ref HEAD` ||
	exit 0 ;# we do not interrupt rebasing detached HEAD
fi

case "$topic" in
refs/heads/??/*)
	;;
*)
	exit 0 ;# we do not interrupt others.
	;;
esac

# Now we are dealing with a topic branch being rebased
# on top of master.  Is it OK to rebase it?

# Does the topic really exist?
git show-ref -q "$topic" || {
	echo >&2 "No such branch $topic"
	exit 1
}

# Is topic fully merged to master?
not_in_master=`git rev-list --pretty=oneline ^master "$topic"`
if test -z "$not_in_master"
then
	echo >&2 "$topic is fully merged to master; better remove it."
	exit 1 ;# we could allow it, but there is no point.
fi

# Is topic ever merged to next?  If so you should not be rebasing it.
only_next_1=`git rev-list ^master "^$topic" ${publish} | sort`
only_next_2=`git rev-list ^master           ${publish} | sort`
if test "$only_next_1" = "$only_next_2"
then
	not_in_topic=`git rev-list "^$topic" master`
	if test -z "$not_in_topic"
	then
		echo >&2 "$topic is already up to date with master"
		exit 1 ;# we could allow it, but there is no point.
	else
		exit 0
	fi
else
	not_in_next=`git rev-list --pretty=oneline ^${publish} "$topic"`
	/usr/bin/perl -e '
		my $topic = $ARGV[0];
		my $msg = "* $topic has commits already merged to public branch:\n";
		my (%not_in_next) = map {
			/^([0-9a-f]+) /;
			($1 => 1);
		} split(/\n/, $ARGV[1]);
		for my $elem (map {
				/^([0-9a-f]+) (.*)$/;
				[$1 => $2];
			} split(/\n/, $ARGV[2])) {
			if (!exists $not_in_next{$elem->[0]}) {
				if ($msg) {
					print STDERR $msg;
					undef $msg;
				}
				print STDERR " $elem->[1]\n";
			}
		}
	' "$topic" "$not_in_next" "$not_in_master"
	exit 1
fi

<<\DOC_END

This sample hook safeguards topic branches that have been
published from being rewound.

The workflow assumed here is:

 * Once a topic branch forks from "master", "master" is never
   merged into it again (either directly or indirectly).

 * Once a topic branch is fully cooked and merged into "master",
   it is deleted.  If you need to build on top of it to correct
   earlier mistakes, a new topic branch is created by forking at
   the tip of the "master".  This is not strictly necessary, but
   it makes it easier to keep your history simple.

 * Whenever you need to test or publish your changes to topic
   branches, merge them into "next" branch.

The script, being an example, hardcodes the publish branch name
to be "next", but it is trivial to make it configurable via
$GIT_DIR/config mechanism.

With this workflow, you would want to know:

(1) ... if a topic branch has ever been merged to "next".  Young
    topic branches can have stupid mistakes you would rather
    clean up before publishing, and things that have not been
    merged into other branches can be easily rebased without
    affecting other people.  But once it is published, you would
    not want to rewind it.

(2) ... if a topic branch has been fully merged to "master".
    Then you can delete it.  More importantly, you should not
    build on top of it -- other people may already want to
    change things related to the topic as patches against your
    "master", so if you need further changes, it is better to
    fork the topic (perhaps with the same name) afresh from the
    tip of "master".

Let's look at this example:

		   o---o---o---o---o---o---o---o---o---o "next"
		  /       /           /           /
		 /   a---a---b A     /           /
		/   /               /           /
	       /   /   c---c---c---c B         /
	      /   /   /             \         /
	     /   /   /   b---b C     \       /
	    /   /   /   /             \     /
    ---o---o---o---o---o---o---o---o---o---o---o "master"


A, B and C are topic branches.

 * A has one fix since it was merged up to "next".

 * B has finished.  It has been fully merged up to "master" and "next",
   and is ready to be deleted.

 * C has not merged to "next" at all.

We would want to allow C to be rebased, refuse A, and encourage
B to be deleted.

To compute (1):

	git rev-list ^master ^topic next
	git rev-list ^master        next

	if these match, topic has not merged in next at all.

To compute (2):

	git rev-list master..topic

	if this is empty, it is fully merged to "master".

DOC_END
````

## File: Frontend/.git/hooks/pre-receive.sample
````
#!/bin/sh
#
# An example hook script to make use of push options.
# The example simply echoes all push options that start with 'echoback='
# and rejects all pushes when the "reject" push option is used.
#
# To enable this hook, rename this file to "pre-receive".

if test -n "$GIT_PUSH_OPTION_COUNT"
then
	i=0
	while test "$i" -lt "$GIT_PUSH_OPTION_COUNT"
	do
		eval "value=\$GIT_PUSH_OPTION_$i"
		case "$value" in
		echoback=*)
			echo "echo from the pre-receive-hook: ${value#*=}" >&2
			;;
		reject)
			exit 1
		esac
		i=$((i + 1))
	done
fi
````

## File: Frontend/.git/hooks/prepare-commit-msg.sample
````
#!/bin/sh
#
# An example hook script to prepare the commit log message.
# Called by "git commit" with the name of the file that has the
# commit message, followed by the description of the commit
# message's source.  The hook's purpose is to edit the commit
# message file.  If the hook fails with a non-zero status,
# the commit is aborted.
#
# To enable this hook, rename this file to "prepare-commit-msg".

# This hook includes three examples. The first one removes the
# "# Please enter the commit message..." help message.
#
# The second includes the output of "git diff --name-status -r"
# into the message, just before the "git status" output.  It is
# commented because it doesn't cope with --amend or with squashed
# commits.
#
# The third example adds a Signed-off-by line to the message, that can
# still be edited.  This is rarely a good idea.

COMMIT_MSG_FILE=$1
COMMIT_SOURCE=$2
SHA1=$3

/usr/bin/perl -i.bak -ne 'print unless(m/^. Please enter the commit message/..m/^#$/)' "$COMMIT_MSG_FILE"

# case "$COMMIT_SOURCE,$SHA1" in
#  ,|template,)
#    /usr/bin/perl -i.bak -pe '
#       print "\n" . `git diff --cached --name-status -r`
# 	 if /^#/ && $first++ == 0' "$COMMIT_MSG_FILE" ;;
#  *) ;;
# esac

# SOB=$(git var GIT_COMMITTER_IDENT | sed -n 's/^\(.*>\).*$/Signed-off-by: \1/p')
# git interpret-trailers --in-place --trailer "$SOB" "$COMMIT_MSG_FILE"
# if test -z "$COMMIT_SOURCE"
# then
#   /usr/bin/perl -i.bak -pe 'print "\n" if !$first_line++' "$COMMIT_MSG_FILE"
# fi
````

## File: Frontend/.git/hooks/push-to-checkout.sample
````
#!/bin/sh

# An example hook script to update a checked-out tree on a git push.
#
# This hook is invoked by git-receive-pack(1) when it reacts to git
# push and updates reference(s) in its repository, and when the push
# tries to update the branch that is currently checked out and the
# receive.denyCurrentBranch configuration variable is set to
# updateInstead.
#
# By default, such a push is refused if the working tree and the index
# of the remote repository has any difference from the currently
# checked out commit; when both the working tree and the index match
# the current commit, they are updated to match the newly pushed tip
# of the branch. This hook is to be used to override the default
# behaviour; however the code below reimplements the default behaviour
# as a starting point for convenient modification.
#
# The hook receives the commit with which the tip of the current
# branch is going to be updated:
commit=$1

# It can exit with a non-zero status to refuse the push (when it does
# so, it must not modify the index or the working tree).
die () {
	echo >&2 "$*"
	exit 1
}

# Or it can make any necessary changes to the working tree and to the
# index to bring them to the desired state when the tip of the current
# branch is updated to the new commit, and exit with a zero status.
#
# For example, the hook can simply run git read-tree -u -m HEAD "$1"
# in order to emulate git fetch that is run in the reverse direction
# with git push, as the two-tree form of git read-tree -u -m is
# essentially the same as git switch or git checkout that switches
# branches while keeping the local changes in the working tree that do
# not interfere with the difference between the branches.

# The below is a more-or-less exact translation to shell of the C code
# for the default behaviour for git's push-to-checkout hook defined in
# the push_to_deploy() function in builtin/receive-pack.c.
#
# Note that the hook will be executed from the repository directory,
# not from the working tree, so if you want to perform operations on
# the working tree, you will have to adapt your code accordingly, e.g.
# by adding "cd .." or using relative paths.

if ! git update-index -q --ignore-submodules --refresh
then
	die "Up-to-date check failed"
fi

if ! git diff-files --quiet --ignore-submodules --
then
	die "Working directory has unstaged changes"
fi

# This is a rough translation of:
#
#   head_has_history() ? "HEAD" : EMPTY_TREE_SHA1_HEX
if git cat-file -e HEAD 2>/dev/null
then
	head=HEAD
else
	head=$(git hash-object -t tree --stdin </dev/null)
fi

if ! git diff-index --quiet --cached --ignore-submodules $head --
then
	die "Working directory has staged changes"
fi

if ! git read-tree -u -m "$commit"
then
	die "Could not update working tree to new HEAD"
fi
````

## File: Frontend/.git/hooks/sendemail-validate.sample
````
#!/bin/sh

# An example hook script to validate a patch (and/or patch series) before
# sending it via email.
#
# The hook should exit with non-zero status after issuing an appropriate
# message if it wants to prevent the email(s) from being sent.
#
# To enable this hook, rename this file to "sendemail-validate".
#
# By default, it will only check that the patch(es) can be applied on top of
# the default upstream branch without conflicts in a secondary worktree. After
# validation (successful or not) of the last patch of a series, the worktree
# will be deleted.
#
# The following config variables can be set to change the default remote and
# remote ref that are used to apply the patches against:
#
#   sendemail.validateRemote (default: origin)
#   sendemail.validateRemoteRef (default: HEAD)
#
# Replace the TODO placeholders with appropriate checks according to your
# needs.

validate_cover_letter () {
	file="$1"
	# TODO: Replace with appropriate checks (e.g. spell checking).
	true
}

validate_patch () {
	file="$1"
	# Ensure that the patch applies without conflicts.
	git am -3 "$file" || return
	# TODO: Replace with appropriate checks for this patch
	# (e.g. checkpatch.pl).
	true
}

validate_series () {
	# TODO: Replace with appropriate checks for the whole series
	# (e.g. quick build, coding style checks, etc.).
	true
}

# main -------------------------------------------------------------------------

if test "$GIT_SENDEMAIL_FILE_COUNTER" = 1
then
	remote=$(git config --default origin --get sendemail.validateRemote) &&
	ref=$(git config --default HEAD --get sendemail.validateRemoteRef) &&
	worktree=$(mktemp --tmpdir -d sendemail-validate.XXXXXXX) &&
	git worktree add -fd --checkout "$worktree" "refs/remotes/$remote/$ref" &&
	git config --replace-all sendemail.validateWorktree "$worktree"
else
	worktree=$(git config --get sendemail.validateWorktree)
fi || {
	echo "sendemail-validate: error: failed to prepare worktree" >&2
	exit 1
}

unset GIT_DIR GIT_WORK_TREE
cd "$worktree" &&

if grep -q "^diff --git " "$1"
then
	validate_patch "$1"
else
	validate_cover_letter "$1"
fi &&

if test "$GIT_SENDEMAIL_FILE_COUNTER" = "$GIT_SENDEMAIL_FILE_TOTAL"
then
	git config --unset-all sendemail.validateWorktree &&
	trap 'git worktree remove -ff "$worktree"' EXIT &&
	validate_series
fi
````

## File: Frontend/.git/hooks/update.sample
````
#!/bin/sh
#
# An example hook script to block unannotated tags from entering.
# Called by "git receive-pack" with arguments: refname sha1-old sha1-new
#
# To enable this hook, rename this file to "update".
#
# Config
# ------
# hooks.allowunannotated
#   This boolean sets whether unannotated tags will be allowed into the
#   repository.  By default they won't be.
# hooks.allowdeletetag
#   This boolean sets whether deleting tags will be allowed in the
#   repository.  By default they won't be.
# hooks.allowmodifytag
#   This boolean sets whether a tag may be modified after creation. By default
#   it won't be.
# hooks.allowdeletebranch
#   This boolean sets whether deleting branches will be allowed in the
#   repository.  By default they won't be.
# hooks.denycreatebranch
#   This boolean sets whether remotely creating branches will be denied
#   in the repository.  By default this is allowed.
#

# --- Command line
refname="$1"
oldrev="$2"
newrev="$3"

# --- Safety check
if [ -z "$GIT_DIR" ]; then
	echo "Don't run this script from the command line." >&2
	echo " (if you want, you could supply GIT_DIR then run" >&2
	echo "  $0 <ref> <oldrev> <newrev>)" >&2
	exit 1
fi

if [ -z "$refname" -o -z "$oldrev" -o -z "$newrev" ]; then
	echo "usage: $0 <ref> <oldrev> <newrev>" >&2
	exit 1
fi

# --- Config
allowunannotated=$(git config --type=bool hooks.allowunannotated)
allowdeletebranch=$(git config --type=bool hooks.allowdeletebranch)
denycreatebranch=$(git config --type=bool hooks.denycreatebranch)
allowdeletetag=$(git config --type=bool hooks.allowdeletetag)
allowmodifytag=$(git config --type=bool hooks.allowmodifytag)

# check for no description
projectdesc=$(sed -e '1q' "$GIT_DIR/description")
case "$projectdesc" in
"Unnamed repository"* | "")
	echo "*** Project description file hasn't been set" >&2
	exit 1
	;;
esac

# --- Check types
# if $newrev is 0000...0000, it's a commit to delete a ref.
zero=$(git hash-object --stdin </dev/null | tr '[0-9a-f]' '0')
if [ "$newrev" = "$zero" ]; then
	newrev_type=delete
else
	newrev_type=$(git cat-file -t $newrev)
fi

case "$refname","$newrev_type" in
	refs/tags/*,commit)
		# un-annotated tag
		short_refname=${refname##refs/tags/}
		if [ "$allowunannotated" != "true" ]; then
			echo "*** The un-annotated tag, $short_refname, is not allowed in this repository" >&2
			echo "*** Use 'git tag [ -a | -s ]' for tags you want to propagate." >&2
			exit 1
		fi
		;;
	refs/tags/*,delete)
		# delete tag
		if [ "$allowdeletetag" != "true" ]; then
			echo "*** Deleting a tag is not allowed in this repository" >&2
			exit 1
		fi
		;;
	refs/tags/*,tag)
		# annotated tag
		if [ "$allowmodifytag" != "true" ] && git rev-parse $refname > /dev/null 2>&1
		then
			echo "*** Tag '$refname' already exists." >&2
			echo "*** Modifying a tag is not allowed in this repository." >&2
			exit 1
		fi
		;;
	refs/heads/*,commit)
		# branch
		if [ "$oldrev" = "$zero" -a "$denycreatebranch" = "true" ]; then
			echo "*** Creating a branch is not allowed in this repository" >&2
			exit 1
		fi
		;;
	refs/heads/*,delete)
		# delete branch
		if [ "$allowdeletebranch" != "true" ]; then
			echo "*** Deleting a branch is not allowed in this repository" >&2
			exit 1
		fi
		;;
	refs/remotes/*,commit)
		# tracking branch
		;;
	refs/remotes/*,delete)
		# delete tracking branch
		if [ "$allowdeletebranch" != "true" ]; then
			echo "*** Deleting a tracking branch is not allowed in this repository" >&2
			exit 1
		fi
		;;
	*)
		# Anything else (is there anything else?)
		echo "*** Update hook: unknown type of update to ref $refname of type $newrev_type" >&2
		exit 1
		;;
esac

# --- Finished
exit 0
````

## File: Frontend/.git/info/exclude
````
# git ls-files --others --exclude-from=.git/info/exclude
# Lines that start with '#' are comments.
# For a project mostly in C, the following would be a good set of
# exclude patterns (uncomment them if you want to use them):
# *.[oa]
# *~
````

## File: Frontend/.git/logs/HEAD
````
0000000000000000000000000000000000000000 3324131b0dd5a90a5485178d1251e140d9ae4aa6 Chalithya <schalithya@gmail.com> 1750788248 -0400	clone: from https://github.com/rajatsachdeva31/ImmiGrowAI-Frontend.git
````

## File: Frontend/.git/logs/refs/heads/main
````
0000000000000000000000000000000000000000 3324131b0dd5a90a5485178d1251e140d9ae4aa6 Chalithya <schalithya@gmail.com> 1750788248 -0400	clone: from https://github.com/rajatsachdeva31/ImmiGrowAI-Frontend.git
````

## File: Frontend/.git/logs/refs/remotes/origin/HEAD
````
0000000000000000000000000000000000000000 3324131b0dd5a90a5485178d1251e140d9ae4aa6 Chalithya <schalithya@gmail.com> 1750788248 -0400	clone: from https://github.com/rajatsachdeva31/ImmiGrowAI-Frontend.git
````

## File: Frontend/.git/packed-refs
````
# pack-refs with: peeled fully-peeled sorted 
3324131b0dd5a90a5485178d1251e140d9ae4aa6 refs/remotes/origin/main
````

## File: Frontend/.git/refs/heads/main
````
3324131b0dd5a90a5485178d1251e140d9ae4aa6
````

## File: Frontend/.git/refs/remotes/origin/HEAD
````
ref: refs/remotes/origin/main
````

## File: Frontend/.gitignore
````
# See https://help.github.com/articles/ignoring-files/ for more about ignoring files.

# dependencies
/node_modules
/.pnp
.pnp.*
.yarn/*
!.yarn/patches
!.yarn/plugins
!.yarn/releases
!.yarn/versions

# testing
/coverage

# next.js
/.next/
/out/

# production
/build

# misc
.DS_Store
*.pem

# debug
npm-debug.log*
yarn-debug.log*
yarn-error.log*
.pnpm-debug.log*

# env files (can opt-in for committing if needed)
.env*

# vercel
.vercel

# typescript
*.tsbuildinfo
next-env.d.ts
````

## File: Frontend/components.json
````json
{
  "$schema": "https://ui.shadcn.com/schema.json",
  "style": "new-york",
  "rsc": true,
  "tsx": true,
  "tailwind": {
    "config": "tailwind.config.ts",
    "css": "src/app/globals.css",
    "baseColor": "zinc",
    "cssVariables": true,
    "prefix": ""
  },
  "aliases": {
    "components": "@/components",
    "utils": "@/lib/utils",
    "ui": "@/components/ui",
    "lib": "@/lib",
    "hooks": "@/hooks"
  },
  "iconLibrary": "lucide"
}
````

## File: Frontend/eslint.config.mjs
````
import { dirname } from "path";
import { fileURLToPath } from "url";
import { FlatCompat } from "@eslint/eslintrc";

const __filename = fileURLToPath(import.meta.url);
const __dirname = dirname(__filename);

const compat = new FlatCompat({
  baseDirectory: __dirname,
});

const eslintConfig = [
  ...compat.extends("next/core-web-vitals", "next/typescript"),
];

export default eslintConfig;
````

## File: Frontend/next.config.ts
````typescript
import type { NextConfig } from "next";

const nextConfig: NextConfig = {
  reactStrictMode: true,
  env: {
    BASE_URL: process.env.BASE_URL, 
  },
};

export default nextConfig;
````

## File: Frontend/package.json
````json
{
  "name": "ImmiGrow-frontend",
  "version": "0.1.0",
  "private": true,
  "scripts": {
    "dev": "next dev --turbopack",
    "build": "next build",
    "start": "next start",
    "lint": "next lint"
  },
  "dependencies": {
    "@heroicons/react": "^2.2.0",
    "@hookform/resolvers": "^3.10.0",
    "@next/env": "^15.2.0",
    "@radix-ui/react-checkbox": "^1.1.3",
    "@radix-ui/react-dialog": "^1.1.6",
    "@radix-ui/react-dropdown-menu": "^2.1.6",
    "@radix-ui/react-label": "^2.1.2",
    "@radix-ui/react-popover": "^1.1.6",
    "@radix-ui/react-radio-group": "^1.2.3",
    "@radix-ui/react-scroll-area": "^1.2.3",
    "@radix-ui/react-select": "^2.1.6",
    "@radix-ui/react-slot": "^1.1.2",
    "@radix-ui/react-tabs": "^1.1.2",
    "@radix-ui/react-toast": "^1.2.5",
    "@shadcn/ui": "^0.0.4",
    "@tanstack/react-query": "^5.68.0",
    "@tanstack/react-table": "^8.21.2",
    "@wojtekmaj/react-hooks": "^1.22.0",
    "axios": "^1.8.3",
    "bcryptjs": "^2.4.3",
    "class-variance-authority": "^0.7.1",
    "clsx": "^2.1.1",
    "crypto-js": "^4.2.0",
    "date-fns": "^3.6.0",
    "firebase": "^11.2.0",
    "js-cookie": "^3.0.5",
    "lucide-react": "^0.474.0",
    "next": "^15.3.4",
    "next-themes": "^0.4.4",
    "pdfjs-dist": "^5.0.375",
    "react": "^19.0.0",
    "react-day-picker": "^9.5.1",
    "react-dom": "^19.0.0",
    "react-hook-form": "^7.54.2",
    "react-icons": "^5.4.0",
    "react-pdf": "^9.2.1",
    "react-router-dom": "^7.4.0",
    "react-select": "^5.10.0",
    "react-slick": "^0.30.3",
    "react-toastify": "^11.0.5",
    "recharts": "^2.15.1",
    "slick-carousel": "^1.8.1",
    "swiper": "^11.2.4",
    "tailwind-merge": "^2.6.0",
    "tailwindcss-animate": "^1.0.7",
    "zod": "^3.24.1"
  },
  "devDependencies": {
    "@eslint/eslintrc": "^3",
    "@types/bcryptjs": "^2.4.6",
    "@types/crypto-js": "^4.2.2",
    "@types/js-cookie": "^3.0.6",
    "@types/node": "^20",
    "@types/react": "^19",
    "@types/react-dom": "^19",
    "@types/react-slick": "^0.23.13",
    "eslint": "^9",
    "eslint-config-next": "15.1.6",
    "postcss": "^8",
    "tailwindcss": "^3.4.1",
    "typescript": "^5"
  },
  "overrides": {
    "react-is": "^19.0.0-rc-69d4b800-20241021"
  }
}
````

## File: Frontend/postcss.config.mjs
````
/** @type {import('postcss-load-config').Config} */
const config = {
  plugins: {
    tailwindcss: {},
  },
};

export default config;
````

## File: Frontend/README.md
````markdown
# Frontend for ImmiGrow.ai

Welcome to the frontend repository of **ImmiGrow.ai**! This project aims to provide a seamless user experience for individuals navigating the immigration process to Canada, the U.S., and the U.K. through AI-driven solutions.

## Table of Contents

1. [About ImmiGrow.ai](#about-immigratexai)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Getting Started](#getting-started)
5. [Folder Structure](#folder-structure)

---

## About ImmiGrow.ai

**ImmiGrow.ai** is a platform that:

- Assists individuals from countries such as India, the Philippines, Sri Lanka, Bangladesh, Pakistan, Nigeria, Cameroon, and Eritrea.
- Provides services to apply for work permits, study permits, and permanent residency without traditional immigration agents.
- Offers innovative solutions like building Canadian credit history before arrival.

Our mission is to make immigration processes accessible, cost-effective, and efficient for everyone.

---

## Features

### For Immigrants

- Budgeting assistance for pre- and post-arrival stages.
- Checklists covering essential tasks like obtaining SIN, health cards, and PR confirmation.
- Search functionality for houses, cars, and other essential services.
- Video calling for virtual tours and consultations.

### For Service Providers

- Account creation and onboarding for Realtors and Car Dealerships.
- Listing management (houses, cars).
- Tenant and buyer document verification.
- Open house announcements and booking requests.
- Insurance and financing calculators.

---

## Tech Stack

### Framework

- **Next.js**: React-based framework for server-side rendering and static site generation.

### Libraries and Tools

- **Tailwind CSS**: Utility-first CSS framework for styling.
- **shadcn/ui**: Component library for design consistency.
- **Framer Motion**: Animations and transitions.
- **lucide-react**: Icon library.

---

## Getting Started

### Prerequisites

- Node.js (>= 16.x)
- npm or yarn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/ImmigrateXai/ImmigrateXai-Frontend.git
   ```

2. Navigate to the project directory:

   ```bash
   cd ImmigrateXai-Frontend
   ```

3. Install dependencies:

   ```bash
   npm install
   # or
   yarn install
   ```

4. Start the development server:

   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. Open your browser and visit:
   ```
   http://localhost:3000
   ```

---

## Folder Structure

```
frontend-ImmiGrow/
├── public/         # Static files and assets
├── src/
   ├── app/         # Application files
   ├── components/  # Reusable components
   └── utils/       # Helper functions and utilities
└── package.json    # Project metadata and dependencies
```

---

### Contact

For questions, feedback, or support, please contact us at [support@ImmiGrow.ai](mailto:admin@ImmiGrow.ai).
````

## File: Frontend/src/app/(auth)/forgot-password/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import Link from "next/link";
import { useState } from "react";
import { FaSpinner } from "react-icons/fa";

const ForgotPassword = () => {
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const [email, setEmail] = useState("");
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);

  const handleForgotPassword = async (
    e: React.MouseEvent<HTMLButtonElement>
  ) => {
    e.preventDefault();
    setLoading(true);
    if (!email) {
      setError("Please fill in all fields");
      setLoading(false);
      return;
    }
    const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    if (!emailPattern.test(email)) {
      setError("Please enter a valid email address");
      setLoading(false);
      return;
    }

    try {
      const response = await fetch(`${endpoint}api/users/forgot-password`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        body: JSON.stringify({ email }),
      });

      const data = await response.json();

      if (!response.ok) {
        setError(data.error);
        return;
      }

      if (data.message) {
        setError(data.message);
      }
    } catch (error) {
      console.error(error);
      setError("Failed to reset password");
    } finally {
      setLoading(false);
    }
  };
  return (
    <div className="h-full md:flex">
      <div className="w-full p-12 h-full flex flex-col justify-center items-center">
        <div className="max-w-md lg:max-w-lg">
          <div className=" py-8 px-6 shadow shadow-muted-foreground rounded-lg sm:px-10 text-center">
            <h2 className="text-3xl font-bold mb-4">Forgot Password?</h2>
            <p className=" mb-8">Enter your email and password below</p>
            <Input
              placeholder="email"
              className="mb-4"
              type="email"
              value={email}
              onChange={(e) => setEmail(e.target.value)}
            />
            <Button
              className={
                "bg-blue-600 hover:bg-blue-500 w-full mb-4" +
                (loading
                  ? " cursor-not-allowed bg-blue-300 hover:bg-blue-300"
                  : "")
              }
              onClick={(e) => handleForgotPassword(e)}
            >
              {loading ? <FaSpinner className="animate-spin" /> : "Verify"}
            </Button>
            {error && <p className="text-red-500 text-sm">{error}</p>}
            <p className="text-md mt-6 pt-6 border-t">
              Remember Password?{" "}
              <Link
                className="text-blue-600 hover:text-blue-500 font-semibold"
                href="/login"
              >
                Login
              </Link>
            </p>
          </div>
        </div>
      </div>
    </div>
  );
};

export default ForgotPassword;
````

## File: Frontend/src/app/(auth)/layout.tsx
````typescript
import Header from "@/components/Header";
import { Toaster } from "@/components/ui/toaster";
import React, { ReactNode } from "react";

async function Layout({ children }: { children: ReactNode }) {

  return (
    <div className="flex flex-col h-screen min-w-full bg-background">
      <Header />
      <main className="w-full h-full">{children}</main>
      <Toaster />
    </div>
  );
}

export default Layout;
````

## File: Frontend/src/app/(auth)/login/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import Link from "next/link";
import { useRouter } from "next/navigation";
import { useState } from "react";
import { FaSpinner } from "react-icons/fa";
import { FcGoogle } from "react-icons/fc";
import CryptoJS from "crypto-js";
import { getAuth, GoogleAuthProvider, signInWithPopup } from "firebase/auth";
import { initializeApp } from "firebase/app";
import { Checkbox } from "@/components/ui/checkbox";
import { Label } from "@/components/ui/label";
import {
  Dialog,
  DialogContent,
  DialogHeader,
  DialogTitle,
  DialogFooter,
} from "@/components/ui/dialog";
import { useToast } from "@/hooks/use-toast";
import Cookies from "js-cookie";
import Image from "next/image";

// Define the UserData interface for checking user verification
interface UserData {
  emailVerified: boolean;
  userVerified: boolean;
  onboarded: boolean;
  userRole?: string;
}

const endpoint = process.env.NEXT_PUBLIC_API_URL;

const Login = () => {
  const [email, setEmail] = useState("");
  const [password, setPassword] = useState("");
  const [rememberMe, setRememberMe] = useState(false);
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);
  const [showDialog, setShowDialog] = useState(false);
  // const [token, setToken] = useState("");
  const { toast } = useToast();

  const router = useRouter();
  const secret = process.env.NEXT_PUBLIC_SECRET_KEY;

  function encryptPassword(password: string) {
    if (!secret) {
      throw new Error("Secret key is not defined");
    }
    const iv = CryptoJS.lib.WordArray.random(16).toString(); // Random IV
    const encrypted = CryptoJS.AES.encrypt(
      password,
      CryptoJS.enc.Utf8.parse(secret),
      {
        iv: CryptoJS.enc.Hex.parse(iv),
        mode: CryptoJS.mode.CBC,
        padding: CryptoJS.pad.Pkcs7,
      }
    );
    return {
      encryptedData: encrypted.ciphertext.toString(CryptoJS.enc.Base64),
      iv: iv,
    };
  }

  const checkUserVerification = (data: UserData) => {
    if (data.onboarded === false) {
      router.push("/onboarding");
      return false;
    } else if (!data.userVerified) {
      router.push("/dashboard/not-verified?reason=user");
      return false;
    } else {
      if (data.userRole === "Car Dealership") {
        router.push("/dashboard/car-dealer");
        return false;
      } else if (data.userRole === "Immigrant") {
        router.push("/dashboard/user");
        return false;
      } else if (data.userRole === "Realtor") {
        router.push("/dashboard/realtor");
        return false;
      } else if (data.userRole === "Immigration Consultant") {
        router.push("/dashboard/consultant");
        return false;
      } else if (data.userRole === "Admin") {
        router.push("/dashboard/admin");
        return false;
      }

      return true;
    }
  };

  const handleLogin = async (e: React.MouseEvent<HTMLButtonElement>) => {
    e.preventDefault();
    setLoading(true);
    setError(""); // Clear any previous errors

    if (!email || !password) {
      setError("Please fill in all fields");
      setLoading(false);
      return;
    }

    const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;

    if (!emailPattern.test(email)) {
      setError("Please enter a valid email address");
      setLoading(false);
      return;
    }

    if (password.length < 6) {
      setError("Password must be at least 6 characters long");
      setLoading(false);
      return;
    }

    const { encryptedData, iv } = encryptPassword(password);

    try {
      const response = await fetch(`${endpoint}api/users/login`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        credentials: "include",
        body: JSON.stringify({ email, password: encryptedData, iv }),
      });

      const data = await response.json();

      if (!response.ok) {
        if (data.emailVerified == false) {
          setError("Please verify your email first");
          // setToken(data.token);
          setShowDialog(true);
          return;
        }
        setError(data.error || "Failed to login");
        return;
      }

      if (data.emailVerified == true) {
        if (rememberMe) {
          localStorage.setItem("email", data.email);
        }
        if (!checkUserVerification(data)) return;
        router.push("/dashboard");
      } else {
        setError(data.message || "Failed to login");
      }
    } catch (error) {
      console.error("Login error:", error);
      setError("Failed to login");
    } finally {
      setLoading(false);
    }
  };

  const handleResendEmail = async () => {
    try {
      await fetch(`${endpoint}api/users/refresh-token`, {
        method: "POST",
        credentials: "include",
      });
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");

      const tokenData = await tokenResponse.json();
      const token = tokenData?.token;
      if (!token) throw new Error("Invalid authentication token");

      await fetch(`${endpoint}api/users/resend-verification`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
      });
      toast({
        title: "Verification email sent",
        description: "Please check your email to verify your account",
      });
      setShowDialog(false);
    } catch (error) {
      console.error("Failed to resend email:", error);
    }
  };

  const firebaseConfig = {
    apiKey: process.env.NEXT_PUBLIC_API_KEY,
    authDomain: process.env.NEXT_PUBLIC_AUTH_DOMAIN,
    projectId: process.env.NEXT_PUBLIC_PROJECT_ID,
  };

  const app = initializeApp(firebaseConfig);

  const handleGoogleLogin = async () => {
    const auth = getAuth(app);
    const provider = new GoogleAuthProvider();
    const rememberMe = false;

    setLoading(true);
    try {
      const result = await signInWithPopup(auth, provider);
      const refreshToken = await result.user.refreshToken;
      const idToken = await result.user.getIdToken();

      const response = await fetch(`${endpoint}api/users/google-signin`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        credentials: "include",
        body: JSON.stringify({ idToken, refreshToken, rememberMe }),
      });

      const data = await response.json();

      if (data) {
        localStorage.setItem("token", idToken);
        if (!checkUserVerification(data)) return;
        router.push("/dashboard");
      } else {
        setError(data.message || "Google Sign-In failed");
      }
    } catch (error) {
      console.error(
        "Error during Google Sign-In or backend communication:",
        error
      );
      setError("Failed to sign up with Google");
    } finally {
      setLoading(false);
    }
  };

  return (
    <>
      <div className="h-full md:flex">
        <div className="md:w-1/2 p-12 h-full flex flex-col justify-center items-center">
          <div className="max-w-md lg:max-w-lg">
            <div className=" py-8 px-6 shadow shadow-muted-foreground rounded-lg sm:px-10 text-center">
              <h2 className="text-3xl font-bold mb-4">Login to your account</h2>
              <p className=" mb-8">Enter your email and password below</p>
              <Input
                placeholder="email"
                className="mb-4"
                type="email"
                value={email}
                onChange={(e) => setEmail(e.target.value)}
              />
              <Input
                placeholder="password"
                className="mb-4"
                type="password"
                value={password}
                onChange={(e) => setPassword(e.target.value)}
              />
              {/* <div className="flex items-center space-x-2 my-4 px-1">
                <Checkbox
                  id="remember"
                  checked={rememberMe}
                  onCheckedChange={(checked) =>
                    setRememberMe(checked ? true : false)
                  }
                />
                <Label
                  htmlFor="remember"
                  className="text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
                >
                  Remember Me
                </Label>
              </div>
              {error && <p className="text-red-500 text-sm">{error}</p>} */}
              <Button
                className={
                  "bg-blue-600 hover:bg-blue-500 w-full mb-4" +
                  (loading
                    ? " cursor-not-allowed bg-blue-300 hover:bg-blue-300"
                    : "")
                }
                onClick={(e) => handleLogin(e)}
              >
                {loading ? <FaSpinner className="animate-spin" /> : "Login"}
              </Button>
              <p className="text-sm mb-4">
                Forgot Password?{" "}
                <Link
                  href={"/forgot-password"}
                  className="font-bold text-blue-600 hover:text-blue-500"
                >
                  Reset
                </Link>
              </p>
              <div className="flex items-center mb-4">
                <div className="flex-grow h-px" />
                <span className="mx-4 text-sm">OR</span>
                <div className="flex-grow h-px" />
              </div>
              <Button
                variant="outline"
                className={
                  "flex items-center justify-center w-full mb-4" +
                  (loading
                    ? " cursor-not-allowed bg-neutral-300 hover:bg-neutral-300"
                    : "")
                }
                onClick={() => handleGoogleLogin()}
              >
                {loading ? (
                  <FaSpinner className="animate-spin" />
                ) : (
                  <>
                    <FcGoogle size={6} /> Continue with Google
                  </>
                )}
              </Button>
              <p className="text-xs mt-4">
                By clicking login, you agree to our Terms of Service and Privacy
                Policy.
              </p>
              <p className="text-md mt-6 pt-6 border-t">
                Don&apos;t have an account?{" "}
                <Link
                  className="text-blue-600 hover:text-blue-500 font-semibold"
                  href="/signup"
                >
                  Sign up
                </Link>
              </p>
            </div>
          </div>
        </div>
        <div className="relative w-1/2 p-12 bg-blue-600 md:flex flex-col justify-between hidden">
          <Image
            src={"/login.jpg"}
            alt="signup"
            layout="fill"
            objectFit="cover"
            className="absolute inset-0 opacity-50"
          />
        </div>
      </div>

      <Dialog open={showDialog} onOpenChange={setShowDialog}>
        <DialogContent>
          <DialogHeader>
            <DialogTitle>Email Verification Required</DialogTitle>
          </DialogHeader>
          <p>Please verify your email to continue.</p>
          <DialogFooter>
            <Button variant="secondary" onClick={() => setShowDialog(false)}>
              Cancel
            </Button>
            <Button onClick={handleResendEmail}>
              Resend Verification Email
            </Button>
          </DialogFooter>
        </DialogContent>
      </Dialog>
    </>
  );
};

export default Login;
````

## File: Frontend/src/app/(auth)/onboarding/car-dealer/BusinessInformation.tsx
````typescript
import React from "react";
import { FormData } from "./types"; // Importing FormData interface
import { Label } from "@/components/ui/label";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import { Checkbox } from "@/components/ui/checkbox";
import {
  Select as SingleSelect,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";
import Select, { MultiValue } from "react-select";

type OptionType = { value: string; label: string };

const carBrandsOptions: OptionType[] = [
  { value: "Brand A", label: "Brand A" },
  { value: "Brand B", label: "Brand B" },
  { value: "Brand C", label: "Brand C" },
  // Add more brands as needed
];

const BusinessInformation: React.FC<{
  formData: FormData; // Use the correct type
  setFormData: React.Dispatch<React.SetStateAction<FormData>>;
  errors: { [key: string]: string }; // Use the correct type
}> = ({ formData, setFormData, errors }) => {
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Business Information</h2>
      <div className="flex justify-between items-center gap-1">
        <Label className="w-1/3">Showroom Location(s):</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.showroomLocations}
          onChange={(e) =>
            setFormData({ ...formData, showroomLocations: e.target.value })
          }
        />
      </div>
      {errors.showroomLocations && <p className="text-red-500 text-sm mb-4">{errors.showroomLocations}</p>}
      <div className="flex justify-between items-center">
        <Label>Test Drive Policy:</Label>
        <Textarea
          className="w-2/3 mb-4"
          value={formData.testDrivePolicy}
          onChange={(e) =>
            setFormData({ ...formData, testDrivePolicy: e.target.value })
          }
        />
      </div>
      {errors.testDrivePolicy && <p className="text-red-500 text-sm mb-4">{errors.testDrivePolicy}</p>}
      <div className="text-left mb-4">
        <p className="mb-2">Vehicle Financing Options:</p>
        <div className="flex justify-between items-center gap-1">
          <div className="flex gap-2">
            <Checkbox
              checked={formData.vehicleFinancingOptions.inHouseFinancing}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  vehicleFinancingOptions: {
                    ...formData.vehicleFinancingOptions,
                    inHouseFinancing: checked ? true : false,
                  },
                })
              }
            />
            <Label>In-house Financing</Label>
          </div>
          
          <div className="flex gap-2">
            <Checkbox
              checked={formData.vehicleFinancingOptions.thirdPartyBanks}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  vehicleFinancingOptions: {
                    ...formData.vehicleFinancingOptions,
                    thirdPartyBanks: checked ? true : false,
                  },
                })
              }
            />
            <Label>Third-Party Banks</Label>
          </div>

          <div className="flex gap-2">
            <Checkbox
              checked={formData.vehicleFinancingOptions.leaseOptions}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  vehicleFinancingOptions: {
                    ...formData.vehicleFinancingOptions,
                    leaseOptions: checked ? true : false,
                  },
                })
              }
            />
            <Label>Lease</Label>
          </div>
          
        </div>
      </div>
      {errors.vehicleFinancingOptions && <p className="text-red-500 text-sm mb-4">{errors.vehicleFinancingOptions}</p>}
      <div className="flex justify-between items-center">
        <Label>Trade-in Options Available:</Label>
        <SingleSelect
          value={formData.tradeInOptions ? "Yes" : "No"}
          onValueChange={(value) =>
            setFormData({
              ...formData,
              tradeInOptions: value === "Yes",
            })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select option" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="Yes">Yes</SelectItem>
            <SelectItem value="No">No</SelectItem>
          </SelectContent>
        </SingleSelect>
      </div>
      <div className="flex justify-between items-center gap-1">
        <Label className="w-1/3">Service & Warranty Information:</Label>
        <Textarea
          className="w-2/3 mb-4"
          value={formData.serviceWarrantyInfo}
          onChange={(e) =>
            setFormData({ ...formData, serviceWarrantyInfo: e.target.value })
          }
        />
      </div>
      {errors.serviceWarrantyInfo && <p className="text-red-500 text-sm mb-4">{errors.serviceWarrantyInfo}</p>}
      <div className="flex justify-between items-center">
        <Label>Registration Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessRegistrationNumber}
          onChange={(e) =>
            setFormData({
              ...formData,
              businessRegistrationNumber: e.target.value,
            })
          }
        />
      </div>
      {errors.businessRegistrationNumber && <p className="text-red-500 text-sm mb-4">{errors.businessRegistrationNumber}</p>}
      <div className="flex justify-between items-center">
        <Label>Business Name:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessName}
          onChange={(e) =>
            setFormData({ ...formData, businessName: e.target.value })
          }
        />
      </div>
      {errors.businessName && <p className="text-red-500 text-sm mb-4">{errors.businessName}</p>}
      <div className="flex justify-between items-center">
        <Label>Business Address:</Label>
        <Textarea
          className="w-2/3 mb-4"
          value={formData.businessAddress}
          onChange={(e) =>
            setFormData({ ...formData, businessAddress: e.target.value })
          }
        />
      </div>
      {errors.businessAddress && <p className="text-red-500 text-sm mb-4">{errors.businessAddress}</p>}
      <div className="flex justify-between items-center">
        <Label>Years in Business:</Label>
        <SingleSelect
          value={formData.yearsInBusiness}
          onValueChange={(value) =>
            setFormData({ ...formData, yearsInBusiness: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select years" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="1-5">1-5 years</SelectItem>
            <SelectItem value="5-10">5-10 years</SelectItem>
            <SelectItem value="10+">10+ years</SelectItem>
          </SelectContent>
        </SingleSelect>
      </div>
      {errors.yearsInBusiness && <p className="text-red-500 text-sm mb-4">{errors.yearsInBusiness}</p>}
      <div className="flex justify-between items-center">
        <Label>Dealership License Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.dealershipLicenseNumber}
          onChange={(e) =>
            setFormData({
              ...formData,
              dealershipLicenseNumber: e.target.value,
            })
          }
        />
      </div>
      {errors.dealershipLicenseNumber && <p className="text-red-500 text-sm mb-4">{errors.dealershipLicenseNumber}</p>}
      <div className="flex justify-between items-center gap-1">
        <Label className="w-1/3">Car Brands Sold:</Label>
        <Select
          isMulti
          options={carBrandsOptions}
          value={
            formData.carBrandsSold?.length
              ? carBrandsOptions.filter((option) =>
                  formData.carBrandsSold?.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              carBrandsSold: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.carBrandsSold && <p className="text-red-500 text-sm mb-4">{errors.carBrandsSold}</p>}
      <div className="text-left mb-4">
        <Label className="w-1/3">New or Used Cars?</Label>
        <div className="flex justify-between items-center gap-1">
          <div className="flex gap-2">
            <Checkbox
              checked={formData.newOrUsedCars.new}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  newOrUsedCars: {
                    ...formData.newOrUsedCars,
                    new: checked ? true : false,
                  },
                })
              }
            />
            <Label className="w-1/3">New</Label>
          </div>
          
          <div className="flex gap-2">
            <Checkbox
              checked={formData.newOrUsedCars.used}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  newOrUsedCars: {
                    ...formData.newOrUsedCars,
                    used: checked ? true : false,
                  },
                })
              }
            />
            <Label className="w-1/3">Used</Label>
          </div>
          
          <div className="flex gap-2">
            <Checkbox
              checked={formData.newOrUsedCars.both}
              onCheckedChange={(checked) =>
                setFormData({
                  ...formData,
                  newOrUsedCars: {
                    ...formData.newOrUsedCars,
                    both: checked ? true : false,
                  },
                })
              }
            />
            <Label className="w-1/3">Both</Label>
          </div>
         
        </div>
      </div>
      {/* {errors.newOrUsedCars && <p className="text-red-500 text-sm mb-4">{errors.newOrUsedCars}</p>} */}
    </div>
  );
};

export default BusinessInformation; // Ensure single default export
````

## File: Frontend/src/app/(auth)/onboarding/car-dealer/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import React, { useState } from "react";
import BusinessInformation from "./BusinessInformation";
// import DocumentUpload from "./DocumentUpload";
import type { FormData } from "./types";
import PersonalInformation from "@/components/onboarding/PersonalInformation";
import TermsAndConditions from "@/components/onboarding/TermsAndConditions";
import DocumentUpload from "@/components/onboarding/DocumentUpload";
import SuccessPage from "./SuccessPage";
import { useRouter } from "next/navigation";

const CarDealer: React.FC = () => {
  const [formData, setFormData] = useState<FormData>({
    fullName: "",
    email: "",
    phoneNumber: "",
    dateOfBirth: "",
    showroomLocations: "",
    testDrivePolicy: "",
    vehicleFinancingOptions: {
      inHouseFinancing: false,
      thirdPartyBanks: false,
      leaseOptions: false,
    },
    tradeInOptions: false,
    serviceWarrantyInfo: "",
    businessRegistrationNumber: "",
    businessName: "",
    businessAddress: "",
    yearsInBusiness: "",
    dealershipLicenseNumber: "",
    carBrandsSold: [],
    newOrUsedCars: {
      new: false,
      used: false,
      both: false,
    },
    governmentId: "",
    licenseDocument: "",
    businessVerification: "",
    backgroundCheckApproved: false,
    termsAccepted: false,
  });

    const [errors, setErrors] = useState({});

  const validateForm = () => {
    const newErrors: Record<string, string> = {};

    if(currentStep===1){
           // Full Name Validation
    if (!formData.fullName || formData.fullName.length < 3) {
      newErrors.fullName = "Full Name must be at least 3 characters";
    }
  
    // Phone Number Validations
    if (!formData.phoneNumber) {
      newErrors.phoneNumber = "Phone number is required";
    } else if (!/^\d+$/.test(formData.phoneNumber)) {
      newErrors.phoneNumber = "Phone number must contain only digits";
    } else if (formData.phoneNumber.length !== 10) {
      newErrors.phoneLength = "Phone number must be exactly 10 digits";
    }
  
    // Date of Birth Validation (Minimum 15 years old)
    if (!formData.dateOfBirth) {
      newErrors.dateOfBirth = "Date of Birth is required";
    } else {
      const dob = new Date(formData.dateOfBirth);
      const today = new Date();
      const minDate = new Date();
      minDate.setFullYear(today.getFullYear() - 15); // 15 years ago
  
      if (dob > minDate) {
        newErrors.dateOfBirth = "You must be at least 15 years old";
      }
    }
    }

    else if(currentStep === 2){

        // Business Name Validation
    // Validate Showroom Location
    if (!formData.showroomLocations) {
      newErrors.showroomLocations = "Showroom Location(s) are required.";
    }
  
    // Validate Test Drive Policy
    if (!formData.testDrivePolicy) {
      newErrors.testDrivePolicy = "Test Drive Policy is required.";
    }
  
    // Validate Vehicle Financing Options (Check at least one option is selected)
    const { inHouseFinancing, thirdPartyBanks, leaseOptions } = formData.vehicleFinancingOptions;
    if (!inHouseFinancing && !thirdPartyBanks && !leaseOptions) {
      newErrors.vehicleFinancingOptions = "At least one vehicle financing option must be selected.";
    }
  
    // Validate Service & Warranty Information
    if (!formData.serviceWarrantyInfo) {
      newErrors.serviceWarrantyInfo = "Service & Warranty Information is required.";
    }
  
    // Validate Business Registration Number
    if (!formData.businessRegistrationNumber) {
      newErrors.businessRegistrationNumber = "Business Registration Number is required.";
    }
  
    // Validate Business Name
    if (!formData.businessName) {
      newErrors.businessName = "Business Name is required.";
    }
  
    // Validate Business Address
    if (!formData.businessAddress) {
      newErrors.businessAddress = "Business Address is required.";
    }
  
    // Validate Years in Business
    if (!formData.yearsInBusiness) {
      newErrors.yearsInBusiness = "Please select years in business.";
    }
  
    // Validate Dealership License Number
    if (!formData.dealershipLicenseNumber) {
      newErrors.dealershipLicenseNumber = "Dealership License Number is required.";
    }
  
    // Validate Car Brands Sold (At least one brand must be selected)
    if (formData.carBrandsSold.length === 0) {
      newErrors.carBrandsSold = "At least one car brand must be selected.";
    }
  
    // Validate New or Used Cars checkboxes (At least one should be checked)
    // const { new: isNew, used: isUsed, both: isBoth } = formData.newOrUsedCars;
    // if (!isNew && !isUsed && !isBoth) {
    //   newErrors.newOrUsedCars = "Please select at least one option (New, Used, or Both).";
    // }
  }


  else if(currentStep===3){
    if (!formData.governmentId) {
      newErrors.governmentId = "Government ID is required.";
    }
    if (!formData.businessVerification) {
      newErrors.businessVerification = "Business verification document is required.";
    }
    if (!formData.licenseDocument) {
      newErrors.licenseDocument = "License document is required.";
    
  }
}
  else if(currentStep===4){
    
    if (formData.backgroundCheckApproved === false) {
      newErrors.backgroundCheckApproved = "Please accept the background verification.";
    }
    if (formData.termsAccepted === false) {
      newErrors.termsAccepted = "Please accept the terms and conditions.";
    }

  }
 

      setErrors(newErrors);
    return Object.keys(newErrors).length === 0;
};

  const [currentStep, setCurrentStep] = useState(1);
  const router = useRouter();

  const handleNextStep = () => {
    // Validate required fields
    if (validateForm()) {
      setCurrentStep((prevStep) => prevStep + 1);
      }
  };

  const handlePreviousStep = () => {
    setCurrentStep((prevStep) => prevStep - 1);
  };

  const [isLoading, setIsLoading] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const handleSubmit = async () => {
    setIsLoading(true);

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      
      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }
      
      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataToSend = new FormData();
      formDataToSend.append("fullName", formData.fullName);
      formDataToSend.append("phoneNo", formData.phoneNumber);
      formDataToSend.append("DOB", formData.dateOfBirth);
      formDataToSend.append("rolename", "Car Dealership");
      formDataToSend.append("businessName", formData.businessName);
      formDataToSend.append("businessAddress", formData.businessAddress);
      formDataToSend.append("businessRegistration", formData.businessRegistrationNumber);
      formDataToSend.append("yearsInBusiness", formData.yearsInBusiness);
      formDataToSend.append("dealershipLicenseNumber", formData.dealershipLicenseNumber);
      formDataToSend.append("carBrandsSold", formData.carBrandsSold.join(","));
      formDataToSend.append("newOrUsedCars", JSON.stringify(formData.newOrUsedCars));
      formDataToSend.append("showroomLocations", formData.showroomLocations);
      formDataToSend.append("testDrivePolicy", formData.testDrivePolicy);
      formDataToSend.append("financingOptions", JSON.stringify(formData.vehicleFinancingOptions));
      formDataToSend.append("tradeInOptions", formData.tradeInOptions.toString());
      formDataToSend.append("serviceWarrantyInfo", formData.serviceWarrantyInfo);
      formDataToSend.append("govId", formData.governmentId);
      formDataToSend.append("licenseCert", formData.licenseDocument);
      formDataToSend.append("businessDoc", formData.businessVerification);
      formDataToSend.append("backgroundVerification", formData.backgroundCheckApproved.toString());
      formDataToSend.append("termsConditionCheck", formData.termsAccepted.toString());

      const response = await fetch(`${endpoint}api/onboarding/information`, {
        method: "POST",
        headers: {
          Authorization: `Bearer ${token}`,
        },
        body: formDataToSend,
      });

      if (!response.ok) {
        const errorData = await response.json();
        throw new Error(errorData.error || "Failed to submit form");
      }

      router.push("/dashboard/not-verified?reason=user");
    } catch (error) {
      console.error("Submission error:", error);
    } finally {
      setIsLoading(false);
    }
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl w-full min-h-[600px] h-full">
        <div className="py-8 px-6 shadow text-center w-full h-full flex flex-col justify-between">
          {currentStep === 1 && (
            <PersonalInformation
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 2 && (
            <BusinessInformation
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 3 && (
            <DocumentUpload formData={formData} setFormData={setFormData}  errors={errors} />
          )}
          {currentStep === 4 && (
            <TermsAndConditions formData={formData} setFormData={setFormData}  errors={errors} />
          )}
          {currentStep === 5 && <SuccessPage formData={formData} />}
          <div className="flex gap-4 justify-center">
            {currentStep > 1 && (
              <Button onClick={handlePreviousStep}>Back</Button>
            )}
            {currentStep == 1 && (
              <Button onClick={() => router.push("/onboarding")}>Back</Button>
            )}
            {currentStep < 5 && <Button onClick={handleNextStep}>Next</Button>}
            {currentStep === 5 && (
              <Button 
                onClick={handleSubmit}
                disabled={isLoading}
              >
                {isLoading ? "Submitting..." : "Submit"}
              </Button>
            )}
          </div>
        </div>
      </div>
    </div>
  );
};

export default CarDealer;
````

## File: Frontend/src/app/(auth)/onboarding/car-dealer/SuccessPage.tsx
````typescript
import React from "react";
import { FormData } from "./types"; // Importing FormData interface

const SuccessPage: React.FC<{ formData: FormData }> = ({ formData }) => {
  return (
    <div className="flex flex-col justify-center">
      <h2 className="text-xl font-semibold mb-2">Review Details</h2>
      <p className="text-center mb-4">
        Please review the details you have provided below.
      </p>
      <span className="flex justify-between mb-1">
        <strong>Full Name:</strong> {formData.fullName}
      </span>
      {/* <span className="flex justify-between mb-1">
        <strong>Email:</strong> {formData.email}
      </span> */}
      <span className="flex justify-between mb-1">
        <strong>Phone Number:</strong> {formData.phoneNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Showroom Location(s):</strong> {formData.showroomLocations}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Test Drive Policy:</strong> {formData.testDrivePolicy}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Trade-in Options:</strong>{" "}
        {formData.tradeInOptions ? "Yes" : "No"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Registration Number:</strong>{" "}
        {formData.businessRegistrationNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Name:</strong> {formData.businessName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Address:</strong> {formData.businessAddress}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Years in Business:</strong> {formData.yearsInBusiness}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Dealership License Number:</strong>{" "}
        {formData.dealershipLicenseNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Car Brands Sold:</strong> {formData.carBrandsSold.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>New or Used Cars:</strong>{" "}
        {formData.newOrUsedCars.new ? "New" : ""}{" "}
        {formData.newOrUsedCars.used ? "Used" : ""}{" "}
        {formData.newOrUsedCars.both ? "Both" : ""}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Government ID:</strong>{" "}
        {formData.governmentId ? "Provided" : "Not provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>License Document:</strong>{" "}
        {formData.licenseDocument ? "Provided" : "Not provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Verification:</strong>{" "}
        {formData.businessVerification ? "Provided" : "Not provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Background Check Approved:</strong>{" "}
        {formData.backgroundCheckApproved? "Yes" : "No"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Terms Accepted:</strong> {formData.termsAccepted ? "Yes" : "No"}
      </span>
    </div>
  );
};

export default SuccessPage;
````

## File: Frontend/src/app/(auth)/onboarding/car-dealer/types.ts
````typescript
export interface FormData {
  fullName: string;
  email: string;
  phoneNumber: string;
  dateOfBirth: string;
  showroomLocations: string;
  testDrivePolicy: string;
  vehicleFinancingOptions: {
    inHouseFinancing: boolean;
    thirdPartyBanks: boolean;
    leaseOptions: boolean;
  };
  tradeInOptions: boolean;
  serviceWarrantyInfo: string;
  businessRegistrationNumber: string;
  businessName: string;
  businessAddress: string;
  yearsInBusiness: string;
  dealershipLicenseNumber: string;
  carBrandsSold: string[];
  newOrUsedCars: {
    new: boolean;
    used: boolean;
    both: boolean;
  };
  governmentId: string | Blob;
  businessVerification: string | Blob;
  licenseDocument: string | Blob;
  backgroundCheckApproved: boolean;
  termsAccepted: boolean;
}
````

## File: Frontend/src/app/(auth)/onboarding/consultant/BusinessInformation.tsx
````typescript
import React from "react";
import { FormData } from "./types";
import { Label } from "@/components/ui/label";
import { Input } from "@/components/ui/input";
import Select, { MultiValue } from "react-select";
import {
  Select as SingleSelect,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";

type OptionType = { value: string; label: string };

const immigrationServicesOptions: OptionType[] = [
  { value: "Permanant Resident", label: "Permanant Resident" },
  { value: "Study Permit", label: "Study Permit" },
  { value: "Work Permit", label: "Work Permit" },
  { value: "Citizen", label: "Citizen" },
];

const languagesSpokenOptions: OptionType[] = [
  { value: "English", label: "Enlish" },
  { value: "French", label: "French" },
  { value: "Hindi", label: "Hindi" },
];

const countriesServedOptions: OptionType[] = [
  { value: "C1", label: "C1" },
  { value: "C2", label: "C2" },
  { value: "C3", label: "C3" },
];

const BusinessInformation: React.FC<{
  formData: FormData;
  setFormData: React.Dispatch<React.SetStateAction<FormData>>;
  errors: { [key: string]: string };
}> = ({ formData, setFormData, errors }) => {
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Business Information</h2>
      <div className="flex justify-between items-center">
        <Label>Business Name:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessName}
          onChange={(e) =>
            setFormData({ ...formData, businessName: e.target.value })
          }
        />
      </div>
      {errors.businessName && (
        <p className="text-red-500 text-sm mb-4">{errors.businessName}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Business Address:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessAddress}
          onChange={(e) =>
            setFormData({ ...formData, businessAddress: e.target.value })
          }
        />
      </div>
      {errors.businessAddress && (
        <p className="text-red-500 text-sm mb-4">{errors.businessAddress}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Registration Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessRegistrationNumber}
          onChange={(e) =>
            setFormData({
              ...formData,
              businessRegistrationNumber: e.target.value,
            })
          }
        />
      </div>
      {errors.businessRegistrationNumber && (
        <p className="text-red-500 text-sm mb-4">
          {errors.businessRegistrationNumber}
        </p>
      )}
      <div className="flex justify-between items-center">
        <Label>Years of Experience:</Label>
        <SingleSelect
          value={formData.yearsOfExperience || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, yearsOfExperience: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select Years of Expereince" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="1-5">1-5 years</SelectItem>
            <SelectItem value="5-10">5-10 years</SelectItem>
            <SelectItem value="10+">10+ years</SelectItem>
          </SelectContent>
        </SingleSelect>
      </div>
      {errors.yearsOfExperience && (
        <p className="text-red-500 text-sm mb-4">{errors.yearsOfExperience}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>License Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.licenseNumber}
          onChange={(e) =>
            setFormData({
              ...formData,
              licenseNumber: e.target.value,
            })
          }
        />
      </div>
      {errors.licenseNumber && (
        <p className="text-red-500 text-sm mb-4">{errors.licenseNumber}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Countries Served:</Label>
        <Select
          isMulti
          options={countriesServedOptions}
          value={
            formData.countriesServed?.length
              ? countriesServedOptions.filter((option) =>
                  formData.countriesServed.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              countriesServed: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.countriesServed && (
        <p className="text-red-500 text-sm mb-4">{errors.countriesServed}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Consultation Fee:</Label>
        <Input
          className="w-2/3 mb-4"
          type="number"
          value={formData.consultationFee}
          onChange={(e) =>
            setFormData({
              ...formData,
              consultationFee: Number(e.target.value),
            })
          }
        />
      </div>
      {errors.consultationFee && (
        <p className="text-red-500 text-sm mb-4">{errors.consultationFee}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Partnered Legal Firms:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.partneredLegalFirms}
          onChange={(e) =>
            setFormData({ ...formData, partneredLegalFirms: e.target.value })
          }
        />
      </div>
      {errors.partneredLegalFirms && (
        <p className="text-red-500 text-sm mb-4">
          {errors.partneredLegalFirms}
        </p>
      )}
      <div className="flex justify-between items-center">
        <Label>Website Links:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.websiteLinks}
          onChange={(e) =>
            setFormData({ ...formData, websiteLinks: e.target.value })
          }
        />
      </div>
      {errors.websiteLinks && (
        <p className="text-red-500 text-sm mb-4">{errors.websiteLinks}</p>
      )}
      <div className="flex justify-between items-center">
        <Label>Immigration Services:</Label>
        <Select
          isMulti
          options={immigrationServicesOptions}
          value={
            formData.immigrationServices?.length
              ? immigrationServicesOptions.filter((option) =>
                  formData.immigrationServices.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              immigrationServices: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.immigrationServices && (
        <p className="text-red-500 text-sm mb-4">
          {errors.immigrationServices}
        </p>
      )}
      <div className="flex justify-between items-center">
        <Label>Languages Spoken:</Label>
        <Select
          isMulti
          options={languagesSpokenOptions}
          value={
            formData.languagesSpoken?.length
              ? languagesSpokenOptions.filter((option) =>
                  formData.languagesSpoken.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              languagesSpoken: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.languagesSpoken && (
        <p className="text-red-500 text-sm mb-4">{errors.languagesSpoken}</p>
      )}
    </div>
  );
};

export default BusinessInformation;
````

## File: Frontend/src/app/(auth)/onboarding/consultant/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button"; // Corrected import statement
import React, { useState } from "react";
import type { FormData } from "./types";
import BusinessInformation from "./BusinessInformation";
import SuccessPage from "./SuccessPage";
import PersonalInformation from "@/components/onboarding/PersonalInformation";
import TermsAndConditions from "@/components/onboarding/TermsAndConditions";
import DocumentUpload from "@/components/onboarding/DocumentUpload";
import { useRouter } from "next/navigation";

const Consultant = () => {
  const [formData, setFormData] = useState<FormData>({
    fullName: "",
    email: "",
    phoneNumber: "",
    dateOfBirth: "",
    countriesServed: [],
    consultationFee: 0,
    businessRegistrationNumber: "",
    partneredLegalFirms: "",
    websiteLinks: "",
    businessName: "",
    businessAddress: "",
    yearsOfExperience: "",
    licenseNumber: "",
    immigrationServices: [],
    languagesSpoken: [],
    governmentId: "",
    businessVerification: "",
    licenseDocument: "",
    backgroundCheckApproved: false,
    termsAccepted: false,
  });

  const [currentStep, setCurrentStep] = useState(1);
  const router = useRouter();

  const [errors, setErrors] = useState({});

  const validateForm = () => {
    const newErrors: Record<string, string> = {};

    if (currentStep === 1) {
      // Full Name Validation
      if (!formData.fullName || formData.fullName.length < 3) {
        newErrors.fullName = "Full Name must be at least 3 characters";
      }

      // Phone Number Validations
      if (!formData.phoneNumber) {
        newErrors.phoneNumber = "Phone number is required";
      } else if (!/^\d+$/.test(formData.phoneNumber)) {
        newErrors.phoneNumber = "Phone number must contain only digits";
      } else if (formData.phoneNumber.length !== 10) {
        newErrors.phoneLength = "Phone number must be exactly 10 digits";
      }

      // Date of Birth Validation (Minimum 15 years old)
      if (!formData.dateOfBirth) {
        newErrors.dateOfBirth = "Date of Birth is required";
      } else {
        const dob = new Date(formData.dateOfBirth);
        const today = new Date();
        const minDate = new Date();
        minDate.setFullYear(today.getFullYear() - 15); // 15 years ago

        if (dob > minDate) {
          newErrors.dateOfBirth = "You must be at least 15 years old";
        }
      }
    } else if (currentStep === 2) {
      // Business Name Validation
      // Validate Business Name
      if (!formData.businessName.trim()) {
        newErrors.businessName = "Business name is required.";
      }

      // Validate Business Address
      if (!formData.businessAddress.trim()) {
        newErrors.businessAddress = "Business address is required.";
      }

      // Validate Registration Number
      if (!formData.businessRegistrationNumber.trim()) {
        newErrors.businessRegistrationNumber =
          "Registration number is required.";
      }

      // Validate Years of Experience (must be a number)
      if (!formData.yearsOfExperience.trim()) {
        newErrors.yearsOfExperience = "Years of experience is required.";
      }

      // Validate License Number
      if (!formData.licenseNumber.trim()) {
        newErrors.licenseNumber = "License number is required.";
      }

      // Validate Countries Served (must have at least one selection)
      if (!formData.countriesServed || formData.countriesServed.length === 0) {
        newErrors.countriesServed = "Please select at least one country.";
      }

      // Validate Consultation Fee (must be a valid number)
      if (!formData.consultationFee) {
        newErrors.consultationFee = "Consultation fee is required.";
      } else if (
        isNaN(Number(formData.consultationFee)) ||
        Number(formData.consultationFee) < 0
      ) {
        newErrors.consultationFee = "Please enter a valid fee.";
      }

      // Validate Partnered Legal Firms
      if (!formData.partneredLegalFirms.trim()) {
        newErrors.partneredLegalFirms = "Please enter partnered legal firms.";
      }

      // Validate Website Links (should be a valid URL)
      if (
        !formData.websiteLinks ||
        (formData.websiteLinks.trim() &&
          !/^https?:\/\/[^\s]+$/.test(formData.websiteLinks))
      ) {
        newErrors.websiteLinks = "Please enter a valid website URL.";
      }

      // Validate Immigration Services (must have at least one selection)
      if (
        !formData.immigrationServices ||
        formData.immigrationServices.length === 0
      ) {
        newErrors.immigrationServices = "Please select at least one service.";
      }

      // Validate Languages Spoken (must have at least one selection)
      if (!formData.languagesSpoken || formData.languagesSpoken.length === 0) {
        newErrors.languagesSpoken = "Please select at least one language.";
      }
    } else if (currentStep === 3) {
      if (!formData.governmentId) {
        newErrors.governmentId = "Government ID is required.";
      }
      if (!formData.businessVerification) {
        newErrors.businessVerification =
          "Business verification document is required.";
      }
      if (!formData.licenseDocument) {
        newErrors.licenseDocument = "License document is required.";
      }
    } else if (currentStep === 4) {
      if (formData.backgroundCheckApproved === false) {
        newErrors.backgroundCheckApproved =
          "Please accept the background verification.";
      }
      if (formData.termsAccepted === false) {
        newErrors.termsAccepted = "Please accept the terms and conditions.";
      }
    }

    setErrors(newErrors);
    return Object.keys(newErrors).length === 0;
  };

  const handleNextStep = () => {
    if (validateForm()) {
      setCurrentStep((prevStep) => prevStep + 1);
    }
  };

  const handlePreviousStep = () => {
    setCurrentStep((prevStep) => prevStep - 1);
  };

  const [isLoading, setIsLoading] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const handleSubmit = async () => {
    setIsLoading(true);

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataToSend = new FormData();
      formDataToSend.append("fullName", formData.fullName);
      formDataToSend.append("phoneNo", formData.phoneNumber);
      formDataToSend.append("DOB", formData.dateOfBirth);
      formDataToSend.append("rolename", "Immigration Consultant");
      formDataToSend.append("businessName", formData.businessName);
      formDataToSend.append("businessAddress", formData.businessAddress);
      formDataToSend.append(
        "businessRegistration",
        formData.businessRegistrationNumber
      );
      formDataToSend.append("yearsOfExperience", formData.yearsOfExperience);
      formDataToSend.append("licenseNumber", formData.licenseNumber);
      formDataToSend.append(
        "countriesServed",
        formData.countriesServed.join(",")
      );
      formDataToSend.append(
        "consultationFee",
        String(formData.consultationFee)
      );
      formDataToSend.append(
        "partneredLegalFirms",
        formData.partneredLegalFirms
      );
      formDataToSend.append("websiteLinks", formData.websiteLinks);
      formDataToSend.append(
        "servicesOffered",
        formData.immigrationServices.join(",")
      );
      formDataToSend.append(
        "languagesSpoken",
        formData.languagesSpoken.join(",")
      );
      formDataToSend.append("govId", formData.governmentId);
      formDataToSend.append("licenseCert", formData.licenseDocument);
      formDataToSend.append("businessDoc", formData.businessVerification);
      formDataToSend.append(
        "backgroundVerification",
        formData.backgroundCheckApproved.toString()
      );
      formDataToSend.append(
        "termsConditionCheck",
        formData.termsAccepted.toString()
      );

      const response = await fetch(`${endpoint}api/onboarding/information`, {
        method: "POST",
        headers: {
          Authorization: `Bearer ${token}`,
        },
        body: formDataToSend,
      });

      if (!response.ok) {
        const errorData = await response.json();
        throw new Error(errorData.error || "Failed to submit form");
      }

      router.push("/dashboard/not-verified?reason=user");
    } catch (error) {
      console.error("Submission error:", error);
    } finally {
      setIsLoading(false);
    }
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl w-full min-h-[600px] h-full">
        <div className="py-8 px-6 shadow text-center w-full h-full flex flex-col justify-between">
          {currentStep === 1 && (
            <div>
              <PersonalInformation
                formData={formData}
                setFormData={setFormData}
                errors={errors}
              />
            </div>
          )}
          {currentStep === 2 && (
            <div>
              <BusinessInformation
                formData={formData}
                setFormData={setFormData}
                errors={errors}
              />
            </div>
          )}
          {currentStep === 3 && (
            <div>
              <DocumentUpload
                formData={formData}
                setFormData={setFormData}
                errors={errors}
              />
            </div>
          )}
          {currentStep === 4 && (
            <div>
              <TermsAndConditions
                formData={formData}
                setFormData={setFormData}
                errors={errors}
              />
            </div>
          )}
          {currentStep === 5 && <SuccessPage formData={formData} />}
          <div className="flex gap-4 justify-center">
            {currentStep == 1 && (
              <Button onClick={() => router.push("/onboarding")}>Back</Button>
            )}
            {currentStep > 1 && (
              <Button onClick={handlePreviousStep}>Back</Button>
            )}
            {currentStep < 5 && <Button onClick={handleNextStep}>Next</Button>}
            {currentStep === 5 && (
              <Button onClick={handleSubmit} disabled={isLoading}>
                {isLoading ? "Submitting..." : "Submit"}
              </Button>
            )}
          </div>
        </div>
      </div>
    </div>
  );
};

export default Consultant;
````

## File: Frontend/src/app/(auth)/onboarding/consultant/SuccessPage.tsx
````typescript
import React from "react";
import { FormData } from "./types";

const SuccessPage: React.FC<{ formData: FormData }> = ({ formData }) => {
  return (
    <div className="flex flex-col justify-center">
      <h2 className="text-xl font-semibold mb-2">Review Details</h2>
      <p className="text-center mb-4">
        Please review the details you have provided below.
      </p>
      <span className="flex justify-between mb-1">
        <strong>Full Name:</strong> {formData.fullName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Email:</strong> {formData.email}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Phone Number:</strong> {formData.phoneNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Date of Birth:</strong> {formData.dateOfBirth}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Countries Served:</strong> {formData.countriesServed.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Consultation Fee:</strong> {formData.consultationFee}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Registration Number:</strong>{" "}
        {formData.businessRegistrationNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Partnered Legal Firms:</strong> {formData.partneredLegalFirms}
      </span>
    
      <span className="flex justify-between mb-1">
        <strong>Website Links:</strong> {formData.websiteLinks}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Name:</strong> {formData.businessName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Address:</strong> {formData.businessAddress}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Years of Experience:</strong> {formData.yearsOfExperience}
      </span>
      <span className="flex justify-between mb-1">
        <strong>License Number:</strong> {formData.licenseNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Immigration Services:</strong>{" "}
        {formData.immigrationServices.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Languages Spoken:</strong> {formData.languagesSpoken.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Government ID:</strong>{" "}
        {formData.governmentId ? "Provided" : "Not Provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Verification:</strong>{" "}
        {formData.businessVerification ? "Provided" : "Not Provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>License Document:</strong>{" "}
        {formData.licenseDocument ? "Provided" : "Not Provided"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Background Check Approved:</strong>{" "}
        {formData.backgroundCheckApproved ? "Yes" : "No"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Terms Accepted:</strong> {formData.termsAccepted ? "Yes" : "No"}
      </span>
    </div>
  );
};

export default SuccessPage;
````

## File: Frontend/src/app/(auth)/onboarding/consultant/types.ts
````typescript
export interface FormData {
  fullName: string;
  email: string;
  phoneNumber: string;
  dateOfBirth: string;
  countriesServed: string[];
  consultationFee: number;
  businessRegistrationNumber: string;
  partneredLegalFirms: string;
  websiteLinks: string;
  businessName: string;
  businessAddress: string;
  yearsOfExperience: string;
  licenseNumber: string;
  immigrationServices: string[];
  languagesSpoken: string[];
  governmentId: string | Blob;
  businessVerification: string | Blob;
  licenseDocument: string | Blob;
  backgroundCheckApproved: boolean;
  termsAccepted: boolean;
}
````

## File: Frontend/src/app/(auth)/onboarding/immigrant/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import { Checkbox } from "@/components/ui/checkbox";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";
import React, { useState } from "react";
import {
  Popover,
  PopoverContent,
  PopoverTrigger,
} from "@/components/ui/popover";
import { CalendarIcon } from "lucide-react";
import { cn } from "@/lib/utils";
import { Calendar } from "@/components/ui/calendar";
import { format } from "date-fns";
import TermsAndConditions from "@/components/onboarding/TermsAndConditions";
import { useRouter } from "next/navigation";

interface FormData {
  fullName: string;
  phoneNumber: string;
  dateOfBirth: string;
  alreadyInCanada: boolean;
  countryOfOrigin: string;
  workSchoolLocation: string;
  statusInCanada: string;
  governmentId: File | null;
  backgroundCheckApproved: boolean;
  termsAccepted: boolean;
}

const Immigrant = () => {
  const [isOpen, setIsOpen] = useState(false);
  const router = useRouter();
  const [currentStep, setCurrentStep] = useState(1);

  const [formData, setFormData] = useState<FormData>({
    fullName: "",
    phoneNumber: "",
    dateOfBirth: "",
    alreadyInCanada: false,
    countryOfOrigin: "",
    workSchoolLocation: "",
    statusInCanada: "",
    governmentId: null,
    backgroundCheckApproved: false,
    termsAccepted: false,
  });

  const [isLoading, setIsLoading] = useState(false);
  const [error, setError] = useState("");
  const [success, setSuccess] = useState(false);

  // const [token, setToken] = useState("");
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const handleNextStep = () => {
    setCurrentStep((prevStep) => prevStep + 1);
  };

  const handlePreviousStep = () => {
    setCurrentStep((prevStep) => prevStep - 1);
  };

  const handleFileChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    if (e.target.files && e.target.files[0]) {
      setFormData({ ...formData, governmentId: e.target.files[0] });
    }
  };

  const validateForm = () => {
    if (!formData.fullName.trim()) {
      setError("Full name is required");
      return false;
    }
    if (!formData.phoneNumber.trim()) {
      setError("Phone number is required");
      return false;
    }
    if (!formData.dateOfBirth) {
      setError("Date of birth is required");
      return false;
    }

    if (!formData.statusInCanada && formData.alreadyInCanada) {
      setError("Status in Canada is required");
      return false;
    }
    if (!formData.countryOfOrigin) {
      setError("Country of Origin is required");
      return false;
    }
    if (!formData.workSchoolLocation && formData.alreadyInCanada) {
      setError("Location is required");
      return false;
    }
    if (!formData.governmentId) {
      setError("Government ID is required");
      return false;
    }
    if (!formData.termsAccepted) {
      setError("You must accept the terms and conditions");
      return false;
    }
    if (!formData.backgroundCheckApproved) {
      setError("You must approve background check");
      return false;
    }
    setError("");
    return true;
  };

  const handleSubmit = async () => {
    if (!validateForm()) return;

    setIsLoading(true);
    setError("");
    setSuccess(false);

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataToSend = new FormData();
      formDataToSend.append("fullName", formData.fullName);
      formDataToSend.append("DOB", formData.dateOfBirth);
      formDataToSend.append("phoneNo", formData.phoneNumber);
      formDataToSend.append(
        "alreadyInCanada",
        formData.alreadyInCanada ? "true" : "false"
      );
      formDataToSend.append("workSchoolLocation", formData.workSchoolLocation);
      formDataToSend.append("countryOfOrigin", formData.countryOfOrigin);
      formDataToSend.append("statusInCanada", formData.statusInCanada);
      formDataToSend.append("rolename", "Immigrant");
      formDataToSend.append(
        "backgroundVerification",
        String(formData.backgroundCheckApproved)
      );

      formDataToSend.append(
        "termsConditionCheck",
        String(formData.termsAccepted)
      );
      if (formData.governmentId) {
        formDataToSend.append("govId", formData.governmentId);
      }

      const response = await fetch(`${endpoint}api/onboarding/information`, {
        method: "POST",
        headers: {
          Authorization: `Bearer ${token}`,
        },
        body: formDataToSend,
      });

      if (!response.ok) {
        const errorData = await response.json();
        throw new Error(errorData.error || "Failed to submit form");
      }

      setSuccess(true);
      router.push("/dashboard/not-verified?reason=user");
    } catch (error) {
      setError(
        error instanceof Error ? error.message : "An unexpected error occurred"
      );
    } finally {
      setIsLoading(false);
    }
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl w-full min-h-[600px] h-full">
        <div className="py-8 px-6 shadow text-center w-full h-full flex flex-col justify-between">
          {currentStep === 1 && (
            <div className="text-left">
              <h2 className="text-xl font-semibold mb-4">
                Personal Information
              </h2>
              <div className="flex justify-between items-center">
                <Label>Full Name:</Label>
                <Input
                  className="w-2/3 mb-4"
                  type="text"
                  value={formData.fullName}
                  onChange={(e) =>
                    setFormData({ ...formData, fullName: e.target.value })
                  }
                />
              </div>
              <div className="flex justify-between items-center">
                <Label>Phone Number:</Label>
                <Input
                  className="w-2/3 mb-4"
                  type="tel"
                  value={formData.phoneNumber}
                  onChange={(e) =>
                    setFormData({ ...formData, phoneNumber: e.target.value })
                  }
                />
              </div>
              <div className="flex justify-between items-center">
                <Label>Date of Birth:</Label>
                <Popover open={isOpen} onOpenChange={setIsOpen}>
                  <PopoverTrigger asChild>
                    <Button
                      variant={"outline"}
                      className={cn(
                        "w-2/3 mb-4",
                        !formData.dateOfBirth && "text-muted-foreground"
                      )}
                    >
                      {formData.dateOfBirth ? (
                        format(new Date(formData.dateOfBirth), "PPP")
                      ) : (
                        <span>Date of Birth</span>
                      )}
                      <CalendarIcon className="ml-auto h-4 w-4 opacity-50" />
                    </Button>
                  </PopoverTrigger>
                  <PopoverContent className="w-auto p-0" align="start">
                    <Calendar
                      mode="single"
                      captionLayout="dropdown"
                      selected={
                        formData.dateOfBirth
                          ? new Date(formData.dateOfBirth)
                          : undefined
                      }
                      onSelect={(date) =>
                        setFormData({
                          ...formData,
                          dateOfBirth: date
                            ? date.toISOString().split("T")[0]
                            : "",
                        })
                      }
                      onDayClick={() => setIsOpen(false)}
                      fromYear={1960}
                      toYear={new Date().getFullYear()}
                    />
                  </PopoverContent>
                </Popover>
              </div>

              <div className="flex justify-between items-center">
                <Label>Country Of Origin:</Label>
                <Input
                  className="w-2/3 mb-4"
                  type="text"
                  value={formData.countryOfOrigin}
                  onChange={(e) =>
                    setFormData({
                      ...formData,
                      countryOfOrigin: e.target.value,
                    })
                  }
                />
              </div>

              <div className="flex mt-2 items-center mb-4">
                <Label htmlFor="alreadyInCanada">Already In Canada:</Label>
                <Checkbox
                  id="alreadyInCanada"
                  className="ml-14"
                  checked={formData.alreadyInCanada}
                  onCheckedChange={(checked) =>
                    setFormData({ ...formData, alreadyInCanada: !!checked })
                  }
                />
              </div>

              {formData.alreadyInCanada === true && (
                <div className="flex justify-between items-center">
                  <Label>Status in Canada:</Label>
                  <Select
                    value={formData.statusInCanada}
                    onValueChange={(value) =>
                      setFormData({ ...formData, statusInCanada: value })
                    }
                  >
                    <SelectTrigger className="w-2/3 mb-4">
                      <SelectValue placeholder="Select Status" />
                    </SelectTrigger>
                    <SelectContent>
                      <SelectItem value="Study Permit">Study Permit</SelectItem>
                      <SelectItem value="Work Permit">Work Permit</SelectItem>
                      <SelectItem value="Permanent Resident">
                        Permanent Resident
                      </SelectItem>
                      <SelectItem value="Citizen">Citizen</SelectItem>
                    </SelectContent>
                  </Select>
                </div>
              )}
              {formData.alreadyInCanada === true && (
                <div className="flex justify-between items-center">
                  <Label>School/Work Location:</Label>
                  <Input
                    className="w-2/3 mb-4"
                    type="text"
                    value={formData.workSchoolLocation}
                    onChange={(e) =>
                      setFormData({
                        ...formData,
                        workSchoolLocation: e.target.value,
                      })
                    }
                  />
                </div>
              )}

              <div className="flex justify-between items-center">
                <Label>Government ID:</Label>
                <Input
                  className="w-2/3 mb-4"
                  type="file"
                  onChange={handleFileChange}
                />
              </div>
            </div>
          )}
          {currentStep === 2 && (
            <TermsAndConditions
              formData={formData}
              setFormData={setFormData}
              errors={{}}
            />
          )}
          {currentStep === 3 && (
            <div>
              <h2 className="text-xl font-semibold mb-2">Review Details</h2>
              <p className="mb-4">
                Please review the details you have provided below.
              </p>
              {error && (
                <div className="mb-4 p-2 bg-red-100 text-red-600 rounded">
                  {error}
                </div>
              )}
              {success && (
                <div className="mb-4 p-2 bg-blue-100 text-blue-600 rounded">
                  Form submitted successfully!
                </div>
              )}
              <span className="flex justify-between mb-1">
                <strong>Full Name:</strong> {formData.fullName}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Phone Number:</strong> {formData.phoneNumber}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Date of Birth:</strong> {formData.dateOfBirth}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Country Of Origin:</strong> {formData.countryOfOrigin}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Already In Canada</strong>{" "}
                {formData.alreadyInCanada ? "Yes" : "No"}
              </span>
              {formData.alreadyInCanada && (
                <span className="flex justify-between mb-1">
                  <strong>Status in Canada:</strong> {formData.statusInCanada}
                </span>
              )}
              {formData.alreadyInCanada && (
                <span className="flex justify-between mb-1">
                  <strong>School/Work Location:</strong>{" "}
                  {formData.workSchoolLocation}
                </span>
              )}
              <span className="flex justify-between mb-1">
                <strong>Status in Canada:</strong> {formData.statusInCanada}
              </span>
              <span className="flex justify-between mb-1">
                <strong>Government ID:</strong>{" "}
                {formData.governmentId ? "Provided" : "Not Provided"}
              </span>
            </div>
          )}

          <div className="flex gap-4 justify-center">
            {currentStep > 1 && (
              <Button onClick={handlePreviousStep}>Back</Button>
            )}
            {currentStep == 1 && (
              <Button onClick={() => router.push("/onboarding")}>Back</Button>
            )}
            {currentStep < 3 && <Button onClick={handleNextStep}>Next</Button>}
            {currentStep === 3 && (
              <Button onClick={handleSubmit} disabled={isLoading}>
                {isLoading ? "Submitting..." : "Submit"}
              </Button>
            )}
          </div>
        </div>
      </div>
    </div>
  );
};

export default Immigrant;
````

## File: Frontend/src/app/(auth)/onboarding/layout.tsx
````typescript
import { getSession } from "@/lib/auth";
import { redirect } from "next/navigation";
import { ReactNode } from "react";

async function Layout({ children }: { children: ReactNode }) {
  const session = await getSession();

  if (!session) {
    redirect("/login");
  }

  return <main className="w-full h-full">{children}</main>;
}

export default Layout;
````

## File: Frontend/src/app/(auth)/onboarding/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";
import { useRouter } from "next/navigation";
import { useState } from "react";
import { FaSpinner } from "react-icons/fa";

const Onboarding = () => {
  const router = useRouter();
  const [loading, setLoading] = useState(false);
  const [error, setError] = useState("");
  const [userType, setUserType] = useState("");

  const handleUserTypeChange = (value: string) => {
    setUserType(value);
  };

  const handleSubmit = () => {
    setLoading(true);
    setError("");

    if (!userType) {
      setError("Please select a user type.");
      setLoading(false);
      return;
    }

    const routeMap: { [key: string]: string } = {
      Realtors: "/onboarding/realtor",
      "Car Dealers": "/onboarding/car-dealer",
      "Immigration Consultants": "/onboarding/consultant",
      Immigrant: "/onboarding/immigrant",
    };

    // Redirect based on user type
    router.push(routeMap[userType]);
    setLoading(false);
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl">
        <div className="py-8 px-6 shadow rounded-lg text-center">
          <h2 className="text-3xl font-bold mb-6">Onboarding Form</h2>
          <div className="flex gap-2"></div>
          <Select onValueChange={handleUserTypeChange}>
            <SelectTrigger className="w-full mb-4">
              <SelectValue placeholder="Select User Type" />
            </SelectTrigger>
            <SelectContent>
              <SelectItem value="Realtors">Realtors</SelectItem>
              <SelectItem value="Car Dealers">Car Dealers</SelectItem>
              <SelectItem value="Immigration Consultants">
                Immigration Consultants
              </SelectItem>
              <SelectItem value="Immigrant">Immigrant</SelectItem>
            </SelectContent>
          </Select>
          <Button
            className={
              "bg-blue-600 hover:bg-blue-500 w-full mb-4" +
              (loading ? " cursor-not-allowed bg-blue-300" : "")
            }
            onClick={handleSubmit}
            disabled={loading}
          >
            {loading ? <FaSpinner className="animate-spin" /> : "Next"}
          </Button>
          {error && <p className="text-red-500 text-sm">{error}</p>}
        </div>
      </div>
    </div>
  );
};

export default Onboarding;
````

## File: Frontend/src/app/(auth)/onboarding/realtor/BusinessInformation.tsx
````typescript
import React from "react";
import { FormData } from "./types";
import { Label } from "@/components/ui/label";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import Select, { MultiValue } from "react-select";
import {
  Select as SingleSelect,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";

type OptionType = { value: string; label: string };

const areasCoveredOptions: OptionType[] = [
  { value: "city", label: "City" },
  { value: "region", label: "Region" },
];

const specialtiesOptions: OptionType[] = [
  { value: "rentals", label: "Rentals" },
  { value: "sales", label: "Sales" },
  { value: "commercial", label: "Commercial" },
  { value: "residential", label: "Residential" },
  { value: "luxury", label: "Luxury Homes" },
];

const BusinessInformation: React.FC<{
  formData: FormData;
  setFormData: React.Dispatch<React.SetStateAction<FormData>>;
  errors: { [key: string]: string }; // Define errors as an object
}> = ({ formData, setFormData, errors }) => {

  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Business Information</h2>
      <div className="flex justify-between items-center">
        <Label>Business Name:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.businessName || ""}
          onChange={(e) =>
            setFormData({ ...formData, businessName: e.target.value })
          }
        />
      </div>
      {errors.businessName && <p className="text-red-500 text-sm mb-4">{errors.businessName}</p>}
      <div className="flex justify-between items-center">
        <Label>Business Address:</Label>
        <Textarea
          className="w-2/3 mb-4"
          value={formData.businessAddress || ""}
          onChange={(e) =>
            setFormData({ ...formData, businessAddress: e.target.value })
          }
        />
      </div>
      {errors.businessAddress && <p className="text-red-500 text-sm mb-4">{errors.businessAddress}</p>}
      <div className="flex justify-between items-center">
        <Label>License Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.licenseNumber || ""}
          onChange={(e) =>
            setFormData({ ...formData, licenseNumber: e.target.value })
          }
        />
      </div>
      {errors.licenseNumber && <p className="text-red-500 text-sm mb-4">{errors.licenseNumber}</p>}
      <div className="flex justify-between items-center">
        <Label>Years of Experience:</Label>
        <SingleSelect
          value={formData.yearsOfExperience || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, yearsOfExperience: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select Years of Expereince" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="1-5">1-5 years</SelectItem>
            <SelectItem value="5-10">5-10 years</SelectItem>
            <SelectItem value="10+">10+ years</SelectItem>
          </SelectContent>
        </SingleSelect>
      </div>
      {errors.yearsOfExperience && <p className="text-red-500 text-sm mb-4">{errors.yearsOfExperience}</p>}
      <div className="flex justify-between items-center">
        <Label>Affiliated Associations:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.affiliatedAssociations || ""}
          onChange={(e) =>
            setFormData({ ...formData, affiliatedAssociations: e.target.value })
          }
        />
      </div>
      {errors.affiliatedAssociations && <p className="text-red-500 text-sm mb-4">{errors.affiliatedAssociations}</p>}
      <div className="flex justify-between items-center">
        <Label>Areas Covered:</Label>
        <Select
          isMulti
          options={areasCoveredOptions}
          value={areasCoveredOptions.filter((option) =>
            formData.areasCovered?.includes(option.value)
          )}
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              areasCovered: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.areasCovered && <p className="text-red-500 text-sm mb-4">{errors.areasCovered}</p>}
      <div className="flex justify-between items-center">
        <Label>Specialties:</Label>
        <Select
          isMulti
          options={specialtiesOptions}
          value={
            formData.specialties?.length
              ? specialtiesOptions.filter((option) =>
                  formData.specialties.includes(option.value)
                )
              : []
          }
          onChange={(selectedOptions: MultiValue<OptionType>) =>
            setFormData({
              ...formData,
              specialties: selectedOptions
                ? selectedOptions.map((option) => option.value)
                : [],
            })
          }
          className="w-2/3 mb-4"
        />
      </div>
      {errors.specialties && <p className="text-red-500 text-sm mb-4">{errors.specialties}</p>}
      <div className="flex justify-between items-center">
        <Label>Portfolio/Website Link:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.portfolioLink || ""}
          onChange={(e) =>
            setFormData({ ...formData, portfolioLink: e.target.value })
          }
        />
      </div>
      {errors.portfolioLinkRequired && <p className="text-red-500 text-sm mb-4">{errors.portfolioLinkRequired}</p>}
      {errors.portfolioLink && <p className="text-red-500 text-sm mb-4">{errors.portfolioLink}</p>}
      <div className="flex justify-between items-center">
        <Label>Registration Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.registrationNumber || ""}
          onChange={(e) =>
            setFormData({ ...formData, registrationNumber: e.target.value })
          }
        />
      </div>
      {errors.registrationNumber && <p className="text-red-500 text-sm mb-4">{errors.registrationNumber}</p>}
    </div>
  );
};

export default BusinessInformation;
````

## File: Frontend/src/app/(auth)/onboarding/realtor/OfficeWorkSetup.tsx
````typescript
import React from "react";
import { FormData } from "./types";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "@/components/ui/select";
import { RadioGroup, RadioGroupItem } from "@/components/ui/radio-group";

const OfficeWorkSetup: React.FC<{
  formData: FormData;
  setFormData: React.Dispatch<React.SetStateAction<FormData>>;
  errors: { [key: string]: string };
}> = ({ formData, setFormData, errors }) => {
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Office & Work Setup</h2>

      <div className="flex justify-between items-center">
        <Label>Work Type:</Label>
        <RadioGroup
          className="flex gap-4  mb-4"
          value={formData.workType || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, workType: value })
          }
        >
          <RadioGroupItem value="brokerage" id="brokerage" />
          <Label htmlFor="brokerage" className="mr-4">
            Brokerage
          </Label>

          <RadioGroupItem value="independent" id="independent" />
          <Label htmlFor="independent">Independent</Label>
        </RadioGroup>
      </div>
      {errors.workType && <p className="text-red-500 text-sm mb-4">{errors.workType}</p>}

      {formData.workType === "brokerage" && (
        <div className="flex justify-between items-center">
          <Label>Brokerage Name:</Label>
          <Input
            type="text"
            className="w-2/3 mb-4"
            value={formData.brokerageName || ""}
            onChange={(e) =>
              setFormData({ ...formData, brokerageName: e.target.value })
            }
          />
        </div>
        
      )}
      {errors.brokerageName && <p className="text-red-500 text-sm mb-4">{errors.brokerageName}</p>}

      <div className="flex justify-between items-center">
        <Label>Office Location:</Label>
        <Select
          value={formData.officeLocationAvailability || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, officeLocationAvailability: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select availability" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="yes">Yes</SelectItem>
            <SelectItem value="no">No</SelectItem>
          </SelectContent>
        </Select>
      </div>
      {errors.officeLocationAvailability && <p className="text-red-500 text-sm mb-4">{errors.officeLocationAvailability}</p>}

      <div className="flex justify-between items-center">
        <Label>Total Team Members:</Label>
        <Input
          type="number"
          className="w-2/3 mb-4"
          value={formData.numberOfTeamMembers || 1}
          onChange={(e) =>
            setFormData({
              ...formData,
              numberOfTeamMembers: parseInt(e.target.value, 10),
            })
          }
        />
      </div>
      
      <div className="flex justify-between items-center">
        <Label>Virtual Property Tour:</Label>
        <Select
          value={formData.virtualTourAvailability || ""}
          onValueChange={(value) =>
            setFormData({ ...formData, virtualTourAvailability: value })
          }
        >
          <SelectTrigger className="w-2/3 mb-4">
            <SelectValue placeholder="Select availability" />
          </SelectTrigger>
          <SelectContent>
            <SelectItem value="yes">Yes</SelectItem>
            <SelectItem value="no">No</SelectItem>
          </SelectContent>
        </Select>
      </div>
      {errors.virtualTourAvailability && <p className="text-red-500 text-sm mb-4">{errors.virtualTourAvailability}</p>}
    </div>
  );
};

export default OfficeWorkSetup;
````

## File: Frontend/src/app/(auth)/onboarding/realtor/page.tsx
````typescript
"use client";

import React, { useState } from "react";
import BusinessInformation from "./BusinessInformation";
import OfficeWorkSetup from "./OfficeWorkSetup";
import SuccessPage from "./SuccessPage";
import type { FormData } from "./types";
import { Button } from "@/components/ui/button";
import PersonalInformation from "@/components/onboarding/PersonalInformation";
import TermsAndConditions from "@/components/onboarding/TermsAndConditions";
import DocumentUpload from "@/components/onboarding/DocumentUpload";
import { useRouter } from "next/navigation";

const Realtor = () => {
  const [currentStep, setCurrentStep] = useState(1);
  const router = useRouter();
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  const [errors, setErrors] = useState({});
  const [isSubmitting, setIsSubmitting] = useState(false);
  const [formData, setFormData] = useState<FormData>({
    fullName: "",
    phoneNumber: "",
    dateOfBirth: "",
    businessName: "",
    businessAddress: "",
    licenseNumber: "",
    yearsOfExperience: "",
    affiliatedAssociations: "",
    areasCovered: [],
    specialties: [],
    portfolioLink: "",
    registrationNumber: "",
    workType: "",
    brokerageName: "",
    officeLocationAvailability: "",
    numberOfTeamMembers: 0,
    virtualTourAvailability: "",
    governmentId: "",
    businessVerification: "",
    licenseDocument: "",
    backgroundCheckApproved: false,
    termsAccepted: false,
  });

  const validateForm = () => {
    const newErrors: Record<string, string> = {};

    if (currentStep === 1) {
      // Full Name Validation
      if (!formData.fullName || formData.fullName.length < 3) {
        newErrors.fullName = "Full Name must be at least 3 characters";
      }

      // Phone Number Validations
      if (!formData.phoneNumber) {
        newErrors.phoneNumber = "Phone number is required";
      } else if (!/^\d+$/.test(formData.phoneNumber)) {
        newErrors.phoneNumber = "Phone number must contain only digits";
      } else if (formData.phoneNumber.length !== 10) {
        newErrors.phoneLength = "Phone number must be exactly 10 digits";
      }

      // Date of Birth Validation (Minimum 15 years old)
      if (!formData.dateOfBirth) {
        newErrors.dateOfBirth = "Date of Birth is required";
      } else {
        const dob = new Date(formData.dateOfBirth);
        const today = new Date();
        const minDate = new Date();
        minDate.setFullYear(today.getFullYear() - 15); // 15 years ago

        if (dob > minDate) {
          newErrors.dateOfBirth = "You must be at least 15 years old";
        }
      }
    } else if (currentStep === 2) {
      // Business Name Validation
      if (!formData.businessName || formData.businessName.trim() === "") {
        newErrors.businessName = "Business name is required.";
      }

      // Business Address Validation
      if (!formData.businessAddress || formData.businessAddress.trim() === "") {
        newErrors.businessAddress = "Business address is required.";
      }

      // License Number Validation
      if (!formData.licenseNumber || formData.licenseNumber.trim() === "") {
        newErrors.licenseNumber = "License number is required.";
      }

      // Years of Experience Validation
      if (!formData.yearsOfExperience) {
        newErrors.yearsOfExperience = "Years of experience is required.";
      }

      // Affiliated Associations Validation
      if (
        !formData.affiliatedAssociations ||
        formData.affiliatedAssociations.trim() === ""
      ) {
        newErrors.affiliatedAssociations =
          "Affiliated associations are required.";
      }

      // Areas Covered Validation (at least one required)
      if (!formData.areasCovered || formData.areasCovered.length === 0) {
        newErrors.areasCovered = "At least one area must be selected.";
      }

      // Specialties Validation (at least one required)
      if (!formData.specialties || formData.specialties.length === 0) {
        newErrors.specialties = "At least one specialty must be selected.";
      }

      if (!formData.portfolioLink) {
        newErrors.portfolioLinkRequired = "Link is required";
      } else if (
        !/^https?:\/\/[^\s$.?#].[^\s]*$/.test(formData.portfolioLink)
      ) {
        newErrors.portfolioLink = "Invalid website link.";
      }

      // Registration Number Validation
      if (
        !formData.registrationNumber ||
        formData.registrationNumber.trim() === ""
      ) {
        newErrors.registrationNumber = "Registration number is required.";
      }
    } else if (currentStep === 3) {
      if (!formData.workType) {
        newErrors.workType = "Work type is required.";
      }

      if (formData.workType === "brokerage" && !formData.brokerageName) {
        newErrors.brokerageName = "Brokerage name is required.";
      }

      if (!formData.officeLocationAvailability) {
        newErrors.officeLocationAvailability =
          "Please select office location availability.";
      }

      if (!formData.virtualTourAvailability) {
        newErrors.virtualTourAvailability =
          "Please select virtual tour availability.";
      }
    } else if (currentStep === 4) {
      if (!formData.governmentId) {
        newErrors.governmentId = "Government ID is required.";
      }
      if (!formData.businessVerification) {
        newErrors.businessVerification =
          "Business verification document is required.";
      }
      if (!formData.licenseDocument) {
        newErrors.licenseDocument = "License document is required.";
      }
    } else if (currentStep === 5) {
      if (formData.backgroundCheckApproved === false) {
        newErrors.backgroundCheckApproved =
          "Please accept the background verification.";
      }
      if (formData.termsAccepted === false) {
        newErrors.termsAccepted = "Please accept the terms and conditions.";
      }
    }

    setErrors(newErrors);
    return Object.keys(newErrors).length === 0;
  };

  const handleNextStep = () => {
    if (validateForm()) {
      setCurrentStep((prevStep) => prevStep + 1);
    }
  };

  const handlePreviousStep = () => {
    setCurrentStep((prevStep) => prevStep - 1);
  };

  const handleSubmit = async () => {
    if (isSubmitting) return; // Prevent multiple submissions
    setIsSubmitting(true);
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataToSend = new FormData();
      formDataToSend.append("fullName", formData.fullName);
      formDataToSend.append("phoneNo", formData.phoneNumber);
      formDataToSend.append("DOB", formData.dateOfBirth);
      formDataToSend.append("rolename", "Realtor");
      formDataToSend.append("businessName", formData.businessName);
      formDataToSend.append("businessAddress", formData.businessAddress);
      formDataToSend.append("realEstateLicenseNumber", formData.licenseNumber);
      formDataToSend.append("experienceYears", formData.yearsOfExperience);
      formDataToSend.append(
        "affiliatedAssociations",
        formData.affiliatedAssociations
      );
      formDataToSend.append("areasCovered", formData.areasCovered.join(","));
      formDataToSend.append("specialties", formData.specialties.join(","));
      formDataToSend.append("portfolioLink", formData.portfolioLink);
      formDataToSend.append("registrationNumber", formData.registrationNumber);
      formDataToSend.append("workType", formData.workType);
      formDataToSend.append("brokerageName", formData.brokerageName);
      formDataToSend.append(
        "officeLocationAvailable",
        String(formData.officeLocationAvailability === "yes")
      );
      formDataToSend.append(
        "teamMembers",
        String(formData.numberOfTeamMembers ?? "")
      );
      formDataToSend.append(
        "virtualPropertyTour",
        String(formData.virtualTourAvailability === "yes")
      );

      formDataToSend.append("govId", formData.governmentId);
      formDataToSend.append("businessDoc", formData.businessVerification);
      formDataToSend.append("licenseCert", formData.licenseDocument);
      formDataToSend.append(
        "backgroundVerification",
        formData.backgroundCheckApproved.toString()
      );
      formDataToSend.append(
        "termsConditionCheck",
        formData.termsAccepted.toString()
      );

      const response = await fetch(`${endpoint}api/onboarding/information`, {
        method: "POST",
        headers: {
          Authorization: `Bearer ${token}`,
        },
        body: formDataToSend,
      });

      const data = await response.json();

      if (response.ok) {
        router.push("/dashboard/not-verified?reason=user");
      } else {
        console.error(
          "Failed to create user and upload documents:",
          data.error
        );
        // Handle error (e.g., show an error message)
      }
    } catch (error) {
      console.error("Error:", error);
      // Handle error (e.g., show an error message)
    } finally {
      setIsSubmitting(false);
    }
  };

  return (
    <div className="h-full flex flex-col justify-center items-center">
      <div className="max-w-md lg:max-w-xl w-full min-h-[600px] h-full">
        <div className="py-8 px-6 shadow text-center w-full h-full flex flex-col justify-between">
          {currentStep === 1 && (
            <PersonalInformation
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 2 && (
            <BusinessInformation
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 3 && (
            <OfficeWorkSetup
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 4 && (
            <DocumentUpload
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 5 && (
            <TermsAndConditions
              formData={formData}
              setFormData={setFormData}
              errors={errors}
            />
          )}
          {currentStep === 6 && <SuccessPage formData={formData} />}
          <div className="flex gap-4 justify-center">
            {currentStep > 1 && (
              <Button onClick={handlePreviousStep}>Back</Button>
            )}
            {currentStep == 1 && (
              <Button onClick={() => router.push("/onboarding")}>Back</Button>
            )}
            {currentStep < 6 && <Button onClick={handleNextStep}>Next</Button>}
            {currentStep === 6 && (
              <Button onClick={handleSubmit} disabled={isSubmitting}>
                {isSubmitting ? "Submitting..." : "Submit"}
              </Button>
            )}
          </div>
        </div>
      </div>
    </div>
  );
};

export default Realtor;
````

## File: Frontend/src/app/(auth)/onboarding/realtor/SuccessPage.tsx
````typescript
import React from "react";
import { FormData } from "./types";

const SuccessPage: React.FC<{ formData: FormData }> = ({ formData }) => {
  return (
    <div className="flex flex-col justify-center">
      <h2 className="text-xl font-semibold mb-2">Review Details</h2>
      <p className="text-center mb-4">
        Please review the details you have provided below.
      </p>
      <span className="flex justify-between mb-1">
        <strong>Full Name:</strong> {formData.fullName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Phone Number:</strong> {formData.phoneNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Date of Birth:</strong> {formData.dateOfBirth}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Name:</strong> {formData.businessName}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Business Address:</strong> {formData.businessAddress}
      </span>
      <span className="flex justify-between mb-1">
        <strong>License Number:</strong> {formData.licenseNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Years of Experience:</strong> {formData.yearsOfExperience}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Affiliated Associations:</strong>{" "}
        {formData.affiliatedAssociations}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Areas Covered:</strong> {formData.areasCovered.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Specialties:</strong> {formData.specialties.join(", ")}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Portfolio Link:</strong> {formData.portfolioLink}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Registration Number:</strong> {formData.registrationNumber}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Background Check Approved:</strong>{" "}
        {formData.backgroundCheckApproved? "Yes" : "No"}
      </span>
      <span className="flex justify-between mb-1">
        <strong>Terms Accepted:</strong> {formData.termsAccepted ? "Yes" : "No"}
      </span>
    </div>
  );
};

export default SuccessPage;
````

## File: Frontend/src/app/(auth)/onboarding/realtor/types.ts
````typescript
export interface FormData {
  fullName: string;
  phoneNumber: string;
  dateOfBirth: string;
  businessName: string;
  businessAddress: string;
  licenseNumber: string;
  yearsOfExperience: string;
  affiliatedAssociations: string;
  areasCovered: string[];
  specialties: string[];
  portfolioLink: string;
  registrationNumber: string;
  workType: string;
  brokerageName: string;
  officeLocationAvailability: string;
  numberOfTeamMembers: number;
  virtualTourAvailability: string;
  governmentId: string | Blob;
  businessVerification: string | Blob;
  licenseDocument: string | Blob;
  backgroundCheckApproved: boolean;
  termsAccepted: boolean;
}
````

## File: Frontend/src/app/(auth)/signup/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import Link from "next/link";
import { useState } from "react";
import { FaSpinner } from "react-icons/fa";
import { FcGoogle } from "react-icons/fc";
import { useRouter } from "next/navigation";
import { useToast } from "@/hooks/use-toast";
import CryptoJS from "crypto-js";
import { getAuth, GoogleAuthProvider, signInWithPopup } from "firebase/auth";
import { initializeApp } from "firebase/app";
import Image from "next/image";

const endpoint = process.env.NEXT_PUBLIC_API_URL;

const Signup = () => {
  const [email, setEmail] = useState("");
  const [password, setPassword] = useState("");
  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);

  const router = useRouter();
  const { toast } = useToast();
  const secret = process.env.NEXT_PUBLIC_SECRET_KEY;

  function encryptPassword(password: string) {
    if (!secret) {
      throw new Error("Secret key is not defined");
    }
    // Generate a random IV and convert it to a hexadecimal string
    const iv = CryptoJS.lib.WordArray.random(16).toString(CryptoJS.enc.Hex);

    // Encrypt the password using AES-256-CBC
    const encrypted = CryptoJS.AES.encrypt(
      password,
      CryptoJS.enc.Utf8.parse(secret), // Parse the secret key as UTF-8
      {
        iv: CryptoJS.enc.Hex.parse(iv), // Parse the IV as hexadecimal
        mode: CryptoJS.mode.CBC, // Use CBC mode
        padding: CryptoJS.pad.Pkcs7, // Use PKCS7 padding
      }
    );

    // Return the encrypted password and IV
    return {
      encryptedData: encrypted.ciphertext.toString(CryptoJS.enc.Base64),
      iv: iv,
    };
  }

  const handleSignup = async (e: React.MouseEvent<HTMLButtonElement>) => {
    e.preventDefault();
    setLoading(true);
    setError(""); // Clear any previous errors

    if (!email || !password) {
      setError("Please fill in all fields");
      setLoading(false);
      return;
    }

    const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    if (!emailPattern.test(email)) {
      setError("Please enter a valid email address");
      setLoading(false);
      return;
    }

    if (password.length < 6) {
      setError("Password must be at least 6 characters long");
      setLoading(false);
      return;
    }

    // Encrypt the password
    const { encryptedData, iv } = encryptPassword(password);

    try {
      // Send encrypted password and IV to the backend
      const response = await fetch(`${endpoint}api/users/signup`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        body: JSON.stringify({ email, password: encryptedData, iv }),
        credentials: "include",
      });

      const data = await response.json();

      if (!response.ok) {
        if (data.error === "EMAIL_EXISTS") {
          setError("Email already exists");
        } else {
          setError(data.error || "Failed to signup");
        }
        return;
      }

      if (data.userId) {
        localStorage.setItem("user", JSON.stringify(data.userId));
        toast({
          title: "Signup success",
          description: "Please verify your email before logging in",
        });
        router.push("/login");
      } else {
        setError(data.error || "Failed to signup");
      }
    } catch (error) {
      console.error("Signup error:", error);
      setError("Failed to signup");
    } finally {
      setLoading(false);
    }
  };

  const firebaseConfig = {
    apiKey: process.env.NEXT_PUBLIC_API_KEY,
    authDomain: process.env.NEXT_PUBLIC_AUTH_DOMAIN,
    projectId: process.env.NEXT_PUBLIC_PROJECT_ID,
  };

  const app = initializeApp(firebaseConfig);

  const handleGoogleSignup = async () => {
    const auth = getAuth(app);
    const provider = new GoogleAuthProvider();

    setLoading(true);
    try {
      const result = await signInWithPopup(auth, provider);

      const idToken = await result.user.getIdToken();
      const response = await fetch(`${endpoint}api/users/google-signin`, {
        method: "POST",
        headers: {
          "Content-Type": "application/json",
        },
        body: JSON.stringify({ idToken }),
      });

      const data = await response.json();

      if (data.user) {
        localStorage.setItem("token", idToken);
        // localStorage.setItem("user", JSON.stringify(data.user));
        router.push("/onboarding");
      } else {
        setError(data.message || "Google Sign-In failed");
      }
    } catch (error) {
      console.error(
        "Error during Google Sign-In or backend communication:",
        error
      );
      setError("Failed to sign up with Google");
    } finally {
      setLoading(false);
    }
  };

  return (
    <div className="h-full md:flex">
      <div className="w-1/2  bg-blue-600 md:flex flex-col justify-between hidden">
        <div className="relative h-full flex flex-col items-center justify-center">
          {/* ✅ Background Image with Overlay */}
          <div className="absolute inset-0 opacity-50">
            <Image
              src={"/signup.jpg"} // 🔹 Ensure the correct image path
              alt="signup"
              layout="fill"
              objectFit="cover"
            />
          </div>
        </div>
      </div>
      <div className="md:w-1/2 p-12 h-full flex flex-col justify-center items-center">
        <div className="max-w-md lg:max-w-lg">
          <div className=" py-8 px-6 shadow shadow-muted-foreground rounded-lg sm:px-10 text-center">
            <h2 className="text-3xl font-bold mb-4">Create an account</h2>
            <p className=" mb-8">
              Enter your email below to create your account
            </p>
            <Input
              placeholder="email"
              className="mb-4"
              type="email"
              value={email}
              onChange={(e) => setEmail(e.target.value)}
            />
            <Input
              placeholder="password"
              className="mb-4"
              type="password"
              value={password}
              onChange={(e) => setPassword(e.target.value)}
            />
            <Button
              className={
                "bg-blue-600 hover:bg-blue-500 w-full mb-4" +
                (loading
                  ? " cursor-not-allowed bg-blue-300 hover:bg-blue-300"
                  : "")
              }
              onClick={(e) => handleSignup(e)}
            >
              {loading ? (
                <FaSpinner className="animate-spin" />
              ) : (
                "Sign up with Email"
              )}
            </Button>
            {error && <p className="text-red-500 text-sm">{error}</p>}
            <div className="flex items-center mb-4">
              <div className="flex-grow h-px" />
              <span className="mx-4 text-sm">OR</span>
              <div className="flex-grow h-px" />
            </div>
            <Button
              variant="outline"
              className={
                "flex items-center justify-center w-full mb-4" +
                (loading
                  ? " cursor-not-allowed bg-neutral-300 hover:bg-neutral-300"
                  : "")
              }
              onClick={() => handleGoogleSignup()}
            >
              {loading ? (
                <FaSpinner className="animate-spin" />
              ) : (
                <>
                  <FcGoogle size={6} /> Continue with Google
                </>
              )}
            </Button>
            <p className="text-xs mt-4">
              By clicking signup, you agree to our Terms of Service and Privacy
              Policy.
            </p>
            <p className="text-md mt-6 pt-6 border-t">
              Already have an account?{" "}
              <Link
                className="text-blue-600 hover:text-blue-500 font-semibold"
                href="/login"
              >
                Login
              </Link>
            </p>
          </div>
        </div>
      </div>
    </div>
  );
};

export default Signup;
````

## File: Frontend/src/app/dashboard/admin/page.tsx
````typescript
"use client";

import { useEffect, useState } from "react";
import { useRouter } from "next/navigation";
import SideCard from "@/components/Sidecard";
import {
  Pie,
  PieChart,
  Cell,
  LineChart,
  Line,
  XAxis,
  CartesianGrid,
  BarChart,
  YAxis,
  Bar,
} from "recharts";
import { TrendingUp } from "lucide-react";

import { Card, CardContent, CardHeader, CardTitle } from "@/components/ui/card";
import {
  ChartConfig,
  ChartContainer,
  ChartLegend,
  ChartLegendContent,
  ChartTooltip,
  ChartTooltipContent,
} from "@/components/ui/chart";

interface AdminStats {
  totalUsers: number;
  verifiedUsers: number;
  unverifiedUsers: number;
  houseListings: number;
  carListings: number;
  noOfImmigrant: number;
  formattedData: { month: string; count: number }[];
  userTypeGraph: { userType: string; count: number }[];
  verificationPieChart: { label: string; value: number }[];
}

export default function AdminDashboard() {
  const [stats, setStats] = useState<AdminStats | null>(null);
  const [error, setError] = useState<string>("");
  const [loading, setLoading] = useState<boolean>(true);
  const router = useRouter();
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const services = ["Dashboard", "User List", "Verify Users"];
  const urls = [
    "/dashboard/admin",
    "/dashboard/admin/user-list",
    "/dashboard/admin/verify-users",
  ];

  useEffect(() => {
    const fetchStats = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;
        if (!token) throw new Error("Invalid token");

        const response = await fetch(`${endpoint}api/admin/dashboard/stats`, {
          headers: { Authorization: `Bearer ${token}` },
        });
        if (!response.ok) throw new Error("Failed to fetch admin stats");

        const data = await response.json();

        setStats(data);
      } catch (err: any) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchStats();
  }, [endpoint]);

  if (loading) return <p className="p-6">Loading admin dashboard...</p>;
  if (error) return <p className="p-6 text-red-500">Error: {error}</p>;

  // Prepare User Type data for Pie Chart
  const userTypeChartData =
    stats?.userTypeGraph?.length > 0
      ? stats.userTypeGraph.map((item, index) => ({
          name: item.userType || "Unknown",
          value: item.count || 0,
          fill: ["#0088FE", "#00C49F", "#FFBB28", "#FF8042", "#AA336A"][
            index % 5
          ],
        }))
      : [];

  // Prepare Verified vs. Non-Verified Users data
  const registrationChartData =
    stats?.verificationPieChart?.length > 0
      ? stats.verificationPieChart.map((item, index) => ({
          name: item.label,
          value: item.value,
          fill: ["#34D399", "#ff5733"][index % 2], // blue for Verified, Red for Unverified
        }))
      : [];

  // Prepare Formatted Data for Line Chart (Monthly User Counts)
  const barChartData =
    stats?.formattedData?.length > 0 ? stats.formattedData : [];

  // Chart Configurations
  const userTypeChartConfig: ChartConfig = userTypeChartData.reduce(
    (acc, item) => {
      acc[item.name] = {
        label: item.name,
        color: item.fill,
      };
      return acc;
    },
    {} as ChartConfig
  );

  const registrationChartConfig: ChartConfig = registrationChartData.reduce(
    (acc, item) => {
      acc[item.name] = {
        label: item.name,
        color: item.fill,
      };
      return acc;
    },
    {} as ChartConfig
  );

  const barChartConfig: ChartConfig = {
    count: {
      label: "Users",
      color: "#3498db", // Blue color
    },
  };

  return (
    <div className="grid grid-cols-12 min-h-screen">
      {/* Sidebar */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Quick Links" urls={urls} />
      </div>

      {/* Main Content */}
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Admin Dashboard</h2>

          {/* Stats & Line Chart Side-by-Side */}
          <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
            {/* Stats */}
            <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
              {[
                { title: "Total Users", value: stats?.totalUsers },
                { title: "Verified Users", value: stats?.verifiedUsers },
                { title: "Unverified Users", value: stats?.unverifiedUsers },
                { title: "Total Immigrants", value: stats?.noOfImmigrant },
                { title: "House Listings", value: stats?.houseListings },
                { title: "Car Listings", value: stats?.carListings },
              ].map((stat, index) => (
                <Card key={index} className="p-4 border rounded shadow">
                  <CardHeader>
                    <CardTitle>{stat.title}</CardTitle>
                  </CardHeader>
                  <CardContent>
                    <p className="text-2xl">{stat.value}</p>
                  </CardContent>
                </Card>
              ))}
            </div>

            {/* Line Chart */}
            <Card>
              <CardHeader>
                <CardTitle>Monthly Users Added</CardTitle>
              </CardHeader>
              <CardContent>
                <ChartContainer config={barChartConfig}>
                  <BarChart data={barChartData} width={500} height={300}>
                    <CartesianGrid strokeDasharray="3 3" stroke="#ddd" />
                    <XAxis
                      dataKey="month"
                      tickLine={false}
                      axisLine={false}
                      tickMargin={8}
                      interval={0} // Ensures all months are shown
                    />
                    <YAxis />
                    <ChartTooltip content={<ChartTooltipContent />} />
                    <Bar dataKey="count" fill="#3498db" barSize={40} />
                  </BarChart>
                </ChartContainer>
              </CardContent>
            </Card>
          </div>

          {/* Pie Charts */}
          <div className="mt-8 grid grid-cols-1 md:grid-cols-2 gap-6">
            <Card>
              <CardHeader>
                <CardTitle>User Type Distribution</CardTitle>
              </CardHeader>
              <CardContent>
                <ChartContainer config={userTypeChartConfig}>
                  <PieChart>
                    <ChartTooltip
                      content={<ChartTooltipContent nameKey="name" />}
                    />
                    <Pie data={userTypeChartData} dataKey="value">
                      {userTypeChartData.map((entry, index) => (
                        <Cell key={`cell-${index}`} fill={entry.fill} />
                      ))}
                    </Pie>
                    <ChartLegend
                      content={<ChartLegendContent nameKey="name" />}
                    />
                  </PieChart>
                </ChartContainer>
              </CardContent>
            </Card>

            <Card>
              <CardHeader>
                <CardTitle>Verified vs. Non-Verified Users</CardTitle>
              </CardHeader>
              <CardContent>
                <ChartContainer config={registrationChartConfig}>
                  <PieChart>
                    <ChartTooltip
                      content={<ChartTooltipContent nameKey="name" />}
                    />
                    <Pie data={registrationChartData} dataKey="value">
                      {registrationChartData.map((entry, index) => (
                        <Cell key={`cell-${index}`} fill={entry.fill} />
                      ))}
                    </Pie>
                    <ChartLegend
                      content={<ChartLegendContent nameKey="name" />}
                    />
                  </PieChart>
                </ChartContainer>
              </CardContent>
            </Card>
          </div>
        </div>
      </div>
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/admin/user-list/page.tsx
````typescript
"use client";

import { useEffect, useState } from "react";
import { useRouter } from "next/navigation";
import SideCard from "@/components/Sidecard";
import {
  ColumnDef,
  ColumnFiltersState,
  VisibilityState,
  flexRender,
  getCoreRowModel,
  getFilteredRowModel,
  getPaginationRowModel,
  useReactTable,
} from "@tanstack/react-table";
import { MoreHorizontal } from "lucide-react";
import { Button } from "@/components/ui/button";
import { Checkbox } from "@/components/ui/checkbox";
import {
  DropdownMenu,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuLabel,
  DropdownMenuTrigger,
} from "@/components/ui/dropdown-menu";
import { Input } from "@/components/ui/input";
import {
  Table,
  TableBody,
  TableCell,
  TableHead,
  TableHeader,
  TableRow,
} from "@/components/ui/table";

export type User = {
  id: string;
  fullName: string;
  email: string;
  phoneNo: string;
  DOB: string;
  firebaseUid: string;
  userVerified: boolean;
  statusInCanada: string | null;
  role: { name: string };
};

export default function UserListPage() {
  const [users, setUsers] = useState<User[]>([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState("");
  const [columnFilters, setColumnFilters] = useState<ColumnFiltersState>([]);
  const [columnVisibility, setColumnVisibility] = useState<VisibilityState>({});
  const [rowSelection, setRowSelection] = useState({});
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  const router = useRouter();

  const services = ["Dashboard", "User List", "Verify Users"];
  const urls = [
    "/dashboard/admin",
    "/dashboard/admin/user-list",
    "/dashboard/admin/verify-users",
  ];

  useEffect(() => {
    const fetchUsers = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });

        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;

        if (!token) throw new Error("Invalid token");

        const response = await fetch(
          `${endpoint}api/admin/user-list/user-details`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!response.ok) throw new Error("Failed to fetch user details");

        const data = await response.json();

        // Extract users array correctly
        const extractedUsers = data?.user ?? [];
        if (!Array.isArray(extractedUsers)) {
          throw new Error(
            `Unexpected API response format: ${JSON.stringify(data, null, 2)}`
          );
        }

        setUsers(extractedUsers);
      } catch (err: any) {
        console.error("Error fetching users:", err.message);
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchUsers();
  }, [endpoint]);

  const columns: ColumnDef<User>[] = [
    {
      id: "select",
      header: ({ table }) => (
        <Checkbox
          checked={
            table.getIsAllPageRowsSelected() ||
            (table.getIsSomePageRowsSelected() && "indeterminate")
          }
          onCheckedChange={(value) => table.toggleAllPageRowsSelected(!!value)}
          aria-label="Select all"
        />
      ),
      cell: ({ row }) => (
        <Checkbox
          checked={row.getIsSelected()}
          onCheckedChange={(value) => row.toggleSelected(!!value)}
          aria-label="Select row"
        />
      ),
      enableSorting: false,
      enableHiding: false,
    },
    {
      accessorKey: "fullName",
      header: "Full Name",
      cell: ({ row }) => <div>{row.getValue("fullName")}</div>,
    },
    {
      accessorKey: "email",
      header: "Email",
      cell: ({ row }) => (
        <div className="lowercase">{row.getValue("email")}</div>
      ),
    },
    {
      accessorKey: "phoneNo",
      header: "Phone Number",
      cell: ({ row }) => <div>{row.getValue("phoneNo")}</div>,
    },
    {
      accessorKey: "DOB",
      header: "Date of Birth",
      cell: ({ row }) => (
        <div>{new Date(row.getValue("DOB")).toLocaleDateString()}</div>
      ),
    },
    {
      accessorKey: "statusInCanada",
      header: "Status in Canada",
      cell: ({ row }) => <div>{row.getValue("statusInCanada") || "N/A"}</div>,
    },
    {
      accessorKey: "userVerified",
      header: "Verified",
      cell: ({ row }) => (
        <div
          className={`font-bold ${
            row.getValue("userVerified") ? "text-blue-600" : "text-red-600"
          }`}
        >
          {row.getValue("userVerified") ? "Yes" : "No"}
        </div>
      ),
    },
    {
      accessorFn: (row) => row.role?.name ?? "Unknown",
      header: "Role",
      cell: ({ row }) => (
        <div className="capitalize">{row.original.role?.name ?? "Unknown"}</div>
      ),
    },
    {
      id: "actions",
      header: "Actions",
      enableHiding: false,
      cell: ({ row }) => {
        const user = row.original;

        return (
          <DropdownMenu>
            <DropdownMenuTrigger asChild>
              <Button variant="ghost" className="h-8 w-8 p-0">
                <span className="sr-only">Open menu</span>
                <MoreHorizontal />
              </Button>
            </DropdownMenuTrigger>
            <DropdownMenuContent align="end">
              <DropdownMenuItem
                onClick={() =>
                  router.push(`/dashboard/admin/view-user/${user.id}`)
                }
              >
                View Details
              </DropdownMenuItem>
            </DropdownMenuContent>
          </DropdownMenu>
        );
      },
    },
  ];

  const table = useReactTable({
    data: users,
    columns,
    getCoreRowModel: getCoreRowModel(),
    getPaginationRowModel: getPaginationRowModel(),
    getFilteredRowModel: getFilteredRowModel(),
    state: {
      columnFilters,
      columnVisibility,
      rowSelection,
    },
    onColumnFiltersChange: setColumnFilters,
    onColumnVisibilityChange: setColumnVisibility,
    onRowSelectionChange: setRowSelection,
  });

  return (
    <div className="grid grid-cols-12 min-h-screen">
      {/* Sidebar */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Admin Links" urls={urls} />
      </div>

      {/* Main Content */}
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">User List</h2>

          {loading && <p className="text-gray-500">Loading users...</p>}
          {error && <p className="text-red-500">{error}</p>}

          {!loading && !error && (
            <>
              {/* Search by Name */}
              <div className="flex items-center py-4">
                <Input
                  placeholder="Search by Name..."
                  value={
                    (table.getColumn("fullName")?.getFilterValue() as string) ??
                    ""
                  }
                  onChange={(event) =>
                    table
                      .getColumn("fullName")
                      ?.setFilterValue(event.target.value)
                  }
                  className="max-w-sm"
                />
              </div>

              {/* User Table */}
              <div className="rounded-md border">
                <Table>
                  <TableHeader>
                    {table.getHeaderGroups().map((headerGroup) => (
                      <TableRow key={headerGroup.id}>
                        {headerGroup.headers.map((header) => (
                          <TableHead key={header.id}>
                            {flexRender(
                              header.column.columnDef.header,
                              header.getContext()
                            )}
                          </TableHead>
                        ))}
                      </TableRow>
                    ))}
                  </TableHeader>
                  <TableBody>
                    {table.getRowModel().rows.length > 0 ? (
                      table.getRowModel().rows.map((row) => (
                        <TableRow key={row.id}>
                          {row.getVisibleCells().map((cell) => (
                            <TableCell key={cell.id}>
                              {flexRender(
                                cell.column.columnDef.cell,
                                cell.getContext()
                              )}
                            </TableCell>
                          ))}
                        </TableRow>
                      ))
                    ) : (
                      <TableRow>
                        <TableCell
                          colSpan={columns.length}
                          className="text-center py-6"
                        >
                          No users found.
                        </TableCell>
                      </TableRow>
                    )}
                  </TableBody>
                </Table>
              </div>
            </>
          )}
        </div>
      </div>
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/admin/verify-users/page.tsx
````typescript
"use client";

import { useEffect, useState } from "react";
import { useRouter } from "next/navigation";
import SideCard from "@/components/Sidecard";
import {
  ColumnDef,
  ColumnFiltersState,
  VisibilityState,
  flexRender,
  getCoreRowModel,
  getFilteredRowModel,
  getPaginationRowModel,
  useReactTable,
} from "@tanstack/react-table";
import { MoreHorizontal } from "lucide-react";
import { Button } from "@/components/ui/button";
import { Checkbox } from "@/components/ui/checkbox";
import {
  DropdownMenu,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuLabel,
  DropdownMenuTrigger,
} from "@/components/ui/dropdown-menu";
import { Input } from "@/components/ui/input";
import {
  Table,
  TableBody,
  TableCell,
  TableHead,
  TableHeader,
  TableRow,
} from "@/components/ui/table";

export type UnverifiedUser = {
  id: string;
  fullName: string;
  email: string;
  phoneNo: string;
  DOB: string;
  firebaseUid: string;
  userVerified: boolean;
  statusInCanada: string | null;
  roleId: number;
  userDocuments: { id: string }[];
};

export default function VerifyUsersPage() {
  const [users, setUsers] = useState<UnverifiedUser[]>([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState("");
  const [columnFilters, setColumnFilters] = useState<ColumnFiltersState>([]);
  const [columnVisibility, setColumnVisibility] = useState<VisibilityState>({});
  const [rowSelection, setRowSelection] = useState({});
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  const router = useRouter();

  const services = ["Dashboard", "User List", "Verify Users"];
  const urls = [
    "/dashboard/admin",
    "/dashboard/admin/user-list",
    "/dashboard/admin/verify-users",
  ];

  useEffect(() => {
    const fetchUnverifiedUsers = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });

        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;

        if (!token) throw new Error("Invalid token");

        const response = await fetch(
          `${endpoint}api/admin/verify/unverified-user`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        const data = await response.json();

        if (response.status === 404) {
          setError("No unverified users found");
        }

        const extractedUsers = data?.user ?? [];
        if (!Array.isArray(extractedUsers)) {
          throw new Error(
            `Unexpected API response format: ${JSON.stringify(data, null, 2)}`
          );
        }

        setUsers(extractedUsers);
      } catch (err: any) {
        console.error("Error fetching unverified users:", err.message);
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchUnverifiedUsers();
  }, [endpoint]);

  const columns: ColumnDef<UnverifiedUser>[] = [
    {
      id: "select",
      header: ({ table }) => (
        <Checkbox
          checked={
            table.getIsAllPageRowsSelected() ||
            (table.getIsSomePageRowsSelected() && "indeterminate")
          }
          onCheckedChange={(value) => table.toggleAllPageRowsSelected(!!value)}
          aria-label="Select all"
        />
      ),
      cell: ({ row }) => (
        <Checkbox
          checked={row.getIsSelected()}
          onCheckedChange={(value) => row.toggleSelected(!!value)}
          aria-label="Select row"
        />
      ),
      enableSorting: false,
      enableHiding: false,
    },
    {
      accessorKey: "fullName",
      header: "Full Name",
      cell: ({ row }) => <div>{row.getValue("fullName")}</div>,
    },
    {
      accessorKey: "email",
      header: "Email",
      cell: ({ row }) => (
        <div className="lowercase">{row.getValue("email")}</div>
      ),
    },
    {
      accessorKey: "phoneNo",
      header: "Phone Number",
      cell: ({ row }) => <div>{row.getValue("phoneNo")}</div>,
    },
    {
      accessorKey: "DOB",
      header: "Date of Birth",
      cell: ({ row }) => (
        <div>{new Date(row.getValue("DOB")).toLocaleDateString()}</div>
      ),
    },
    {
      accessorKey: "statusInCanada",
      header: "Status in Canada",
      cell: ({ row }) => <div>{row.getValue("statusInCanada") || "N/A"}</div>,
    },
    {
      accessorKey: "userVerified",
      header: "Verified",
      cell: ({ row }) => (
        <div
          className={`font-bold ${
            row.getValue("userVerified") ? "text-blue-600" : "text-red-600"
          }`}
        >
          {row.getValue("userVerified") ? "Yes" : "No"}
        </div>
      ),
    },
    {
      id: "actions",
      header: "Actions",
      enableHiding: false,
      cell: ({ row }) => {
        const user = row.original;

        return (
          <DropdownMenu>
            <DropdownMenuTrigger asChild>
              <Button variant="ghost" className="h-8 w-8 p-0">
                <span className="sr-only">Open menu</span>
                <MoreHorizontal />
              </Button>
            </DropdownMenuTrigger>
            <DropdownMenuContent align="end">
              <DropdownMenuLabel>Actions</DropdownMenuLabel>
              <DropdownMenuItem
                onClick={() =>
                  router.push(`/dashboard/admin/view-user/${user.id}`)
                }
              >
                View User
              </DropdownMenuItem>
            </DropdownMenuContent>
          </DropdownMenu>
        );
      },
    },
  ];

  const table = useReactTable({
    data: users,
    columns,
    getCoreRowModel: getCoreRowModel(),
    getPaginationRowModel: getPaginationRowModel(),
    getFilteredRowModel: getFilteredRowModel(),
    state: {
      columnFilters,
      columnVisibility,
      rowSelection,
    },
    onColumnFiltersChange: setColumnFilters,
    onColumnVisibilityChange: setColumnVisibility,
    onRowSelectionChange: setRowSelection,
  });

  return (
    <div className="grid grid-cols-12 min-h-screen">
      {/* Sidebar */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Admin Links" urls={urls} />
      </div>

      {/* Main Content */}
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Non-Verified Users</h2>

          {loading && <p className="text-gray-500">Loading users...</p>}
          {error && <p className="text-red-500">{error}</p>}

          {!loading && !error && (
            <>
              {/* Search by Name */}
              <div className="flex items-center py-4">
                <Input
                  placeholder="Search by Name..."
                  value={
                    (table.getColumn("fullName")?.getFilterValue() as string) ??
                    ""
                  }
                  onChange={(event) =>
                    table
                      .getColumn("fullName")
                      ?.setFilterValue(event.target.value)
                  }
                  className="max-w-sm"
                />
              </div>

              {/* User Table */}
              <div className="rounded-md border">
                <Table>
                  <TableHeader>
                    {table.getHeaderGroups().map((headerGroup) => (
                      <TableRow key={headerGroup.id}>
                        {headerGroup.headers.map((header) => (
                          <TableHead key={header.id}>
                            {flexRender(
                              header.column.columnDef.header,
                              header.getContext()
                            )}
                          </TableHead>
                        ))}
                      </TableRow>
                    ))}
                  </TableHeader>
                  <TableBody>
                    {table.getRowModel().rows.length > 0 ? (
                      table.getRowModel().rows.map((row) => (
                        <TableRow key={row.id}>
                          {row.getVisibleCells().map((cell) => (
                            <TableCell key={cell.id}>
                              {flexRender(
                                cell.column.columnDef.cell,
                                cell.getContext()
                              )}
                            </TableCell>
                          ))}
                        </TableRow>
                      ))
                    ) : (
                      <TableRow>
                        <TableCell
                          colSpan={columns.length}
                          className="text-center py-6"
                        >
                          No users found.
                        </TableCell>
                      </TableRow>
                    )}
                  </TableBody>
                </Table>
              </div>
            </>
          )}
        </div>
      </div>
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/admin/view-user/[id]/page.tsx
````typescript
"use client";

import { useEffect, useState } from "react";
import { useParams, useRouter } from "next/navigation";
import { Document, Page, pdfjs } from "react-pdf";
import "react-pdf/dist/esm/Page/AnnotationLayer.css";
import "react-pdf/dist/esm/Page/TextLayer.css";

// Load PDF.js worker locally
pdfjs.GlobalWorkerOptions.workerSrc = `//unpkg.com/pdfjs-dist@${pdfjs.version}/build/pdf.worker.min.mjs`;

type UserDetail = {
  id: number;
  fullName: string;
  email: string;
  phoneNo: string;
  DOB: string;
  firebaseUid: string;
  userVerified: boolean;
  statusInCanada: string | null;
  roleId: number;
  userDocuments: { id: number }[];
  userType: string;
  // Realtor details from Prisma model
  realtor?: {
    businessName: string;
    businessAddress?: string;
    realEstateLicenseNumber: string;
    affiliatedAssociations?: string;
    areasCovered: string;
    specialties: string;
    portfolioWebsite?: string;
    businessRegistration: string;
    workType: string;
    brokerageName?: string;
    officeLocationAvailable: boolean;
    teamMembers: number;
    virtualPropertyTour: boolean;
    yearsOfExperience: string;
  };
  // Car Dealership details from Prisma model
  carDealership?: {
    showroomLocations: string;
    testDrivePolicy: string;
    financingOptions: string;
    tradeInAvailable: boolean;
    serviceWarrantyInfo: string;
    businessRegistration: string;
    businessName: string;
    yearsInBusiness: string;
    dealershipLicenseNumber: string;
    carBrandsSold: string;
    newOrUsedCars: string;
  };
  // Immigration Consultant details from Prisma model
  immigrationConsultant?: {
    countriesServed: string;
    consultationFee: number | null;
    businessRegistration: string;
    partneredLegalFirms?: string;
    websiteOrSocialMedia?: string;
    businessName: string;
    businessAddress: string;
    licenseNumber: string;
    servicesOffered: string;
    languagesSpoken: string;
    yearsOfExperience: string;
  };
};

export default function ViewUserPage() {
  const { id: userId } = useParams();
  const router = useRouter();
  const [user, setUser] = useState<UserDetail | null>(null);
  const [step, setStep] = useState(1);
  const [selectedDocId, setSelectedDocId] = useState<number | null>(null);
  const [documentUrl, setDocumentUrl] = useState<string | null>(null);
  const [numPages, setNumPages] = useState<number | null>(null);
  const [currentPage, setCurrentPage] = useState(1);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState("");
  const [showModal, setShowModal] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const handleBack = () => router.push("/dashboard/admin/user-list");

  // Reset current page when step changes
  useEffect(() => {
    setCurrentPage(1);
  }, [step]);

  // Fetch user details on mount
  useEffect(() => {
    if (!userId || !endpoint) {
      setError("Missing userId or API endpoint.");
      setLoading(false);
      return;
    }
    async function fetchUserDetails() {
      try {
        const token = await fetchAuthToken();
        if (!token) throw new Error("Invalid token received");
        const response = await fetch(
          `${endpoint}api/admin/user-list/user-details/${userId}`,
          { headers: { Authorization: `Bearer ${token}` } }
        );
        if (!response.ok) throw new Error("Failed to fetch user details");
        const data = await response.json();
        setUser(data.user);
        // For step 1, if a document exists, select the first one
        if (data.user.userDocuments.length > 0) {
          setSelectedDocId(data.user.userDocuments[0].id);
        }
      } catch (err: any) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    }
    fetchUserDetails();
  }, [userId, endpoint]);

  // Update selected document when step changes
  useEffect(() => {
    if (!user) {
      setSelectedDocId(null);
      return;
    }
    // If fewer documents than the step number exist, clear the selection
    if (user.userDocuments.length < step) {
      setSelectedDocId(null);
    } else {
      if (step === 1) setSelectedDocId(user.userDocuments[0].id);
      else if (step === 2) setSelectedDocId(user.userDocuments[1].id);
      else if (step === 3) setSelectedDocId(user.userDocuments[2].id);
    }
  }, [step, user]);

  // Fetch PDF when selectedDocId changes
  useEffect(() => {
    if (selectedDocId) {
      fetchUserDocument(selectedDocId);
    } else {
      setDocumentUrl(null);
    }
  }, [selectedDocId]);

  async function fetchAuthToken(): Promise<string | null> {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");
      const tokenData = await tokenResponse.json();
      return tokenData.token;
    } catch (err: any) {
      return null;
    }
  }

  async function fetchUserDocument(documentId: number): Promise<void> {
    try {
      const token = await fetchAuthToken();
      if (!token) throw new Error("Invalid token received");
      // Revoke previous URL if exists
      if (documentUrl) URL.revokeObjectURL(documentUrl);
      const docUrl = `${endpoint}api/admin/user-list/user-document/${documentId}`;
      const response = await fetch(docUrl, {
        method: "GET",
        headers: {
          Authorization: `Bearer ${token}`,
          Accept: "application/pdf",
        },
      });
      if (!response.ok) throw new Error("Failed to fetch document");
      const blob = await response.blob();
      setDocumentUrl(URL.createObjectURL(blob));
    } catch (err: any) {
      setDocumentUrl(null);
    }
  }

  const handleVerifyUser = async (userId: string) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const response = await fetch(`${endpoint}api/admin/verify/verify-user`, {
        method: "PUT",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
        body: JSON.stringify({ id: userId }),
      });

      if (!response.ok) throw new Error("Failed to verify user");

      alert("User has been successfully verified!");

      router.push("/dashboard/admin/user-list");
    } catch (err: any) {
      console.error("Error verifying user:", err.message);
      alert("Failed to verify user. Please try again.");
    }
  };

  if (loading) return <div className="p-5">Loading user details...</div>;
  if (error) return <div className="p-5 text-red-600">Error: {error}</div>;

  // Helper: PDF Viewer with navigation buttons and a key to force re-mounting
  const renderPDFViewer = (title: string) => (
    <div className="p-5 border rounded shadow-sm">
      <h2 className="text-2xl font-bold mb-4">{title}</h2>
      {documentUrl ? (
        <div onContextMenu={(e) => e.preventDefault()} className="border p-3">
          <Document
            key={`doc-${step}-${selectedDocId}`}
            file={documentUrl}
            onLoadSuccess={({ numPages }) => setNumPages(numPages)}
          >
            <Page
              pageNumber={currentPage}
              renderTextLayer={false}
              renderAnnotationLayer={false}
            />
          </Document>
          <div className="flex justify-center space-x-2 mt-2">
            <button
              onClick={() => setCurrentPage((prev) => Math.max(prev - 1, 1))}
              disabled={currentPage <= 1}
              className="px-3 py-1 bg-gray-200 rounded disabled:opacity-50"
            >
              Previous
            </button>
            <span>
              {currentPage} of {numPages}
            </span>
            <button
              onClick={() =>
                setCurrentPage((prev) => Math.min(prev + 1, numPages || 1))
              }
              disabled={numPages === null || currentPage >= (numPages || 1)}
              className="px-3 py-1 bg-gray-200 rounded disabled:opacity-50"
            >
              Next
            </button>
          </div>
        </div>
      ) : (
        <p>No document available.</p>
      )}
    </div>
  );

  // Render step content in a 50/50 layout
  const renderStepContent = () => {
    if (step === 1) {
      return (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {/* Left: User Details */}
          <div className="p-5 border rounded shadow-sm">
            <h2 className="text-2xl font-bold mb-4">User Details</h2>
            <p>
              <strong>Name:</strong> {user?.fullName}
            </p>
            <p>
              <strong>Email:</strong> {user?.email}
            </p>
            <p>
              <strong>Phone:</strong> {user?.phoneNo}
            </p>
            <p>
              <strong>Date of Birth:</strong>{" "}
              {new Date(user?.DOB || "").toLocaleDateString()}
            </p>
            <p>
              <strong>Status in Canada:</strong> {user?.statusInCanada || "N/A"}
            </p>
            <p>
              <strong>Verified:</strong> {user?.userVerified ? "Yes" : "No"}
            </p>
          </div>
          {/* Right: Government ID PDF */}
          {renderPDFViewer("Government ID")}
        </div>
      );
    } else if (step === 2) {
      return (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {/* Left: Business Details */}
          <div className="p-5 border rounded shadow-sm">
            <h2 className="text-2xl font-bold mb-4">Business Details</h2>
            {user.realtor ? (
              <>
                <p>
                  <strong>Business Name:</strong> {user.realtor.businessName}
                </p>
                <p>
                  <strong>Business Address:</strong>{" "}
                  {user.realtor.businessAddress || "N/A"}
                </p>
                <p>
                  <strong>Real Estate License Number:</strong>{" "}
                  {user.realtor.realEstateLicenseNumber}
                </p>
                <p>
                  <strong>Affiliated Associations:</strong>{" "}
                  {user.realtor.affiliatedAssociations || "N/A"}
                </p>
                <p>
                  <strong>Areas Covered:</strong> {user.realtor.areasCovered}
                </p>
                <p>
                  <strong>Specialties:</strong> {user.realtor.specialties}
                </p>
                <p>
                  <strong>Portfolio Website:</strong>{" "}
                  {user.realtor.portfolioWebsite ? (
                    <a
                      href={user.realtor.portfolioWebsite}
                      target="_blank"
                      rel="noopener noreferrer"
                      className="text-blue-600 underline"
                    >
                      {user.realtor.portfolioWebsite}
                    </a>
                  ) : (
                    "N/A"
                  )}
                </p>
                <p>
                  <strong>Business Registration:</strong>{" "}
                  {user.realtor.businessRegistration}
                </p>
                <p>
                  <strong>Work Type:</strong> {user.realtor.workType}
                </p>
                <p>
                  <strong>Brokerage Name:</strong>{" "}
                  {user.realtor.brokerageName || "N/A"}
                </p>
                <p>
                  <strong>Office Location Available:</strong>{" "}
                  {user.realtor.officeLocationAvailable ? "Yes" : "No"}
                </p>
                <p>
                  <strong>Team Members:</strong> {user.realtor.teamMembers}
                </p>
                <p>
                  <strong>Virtual Property Tour:</strong>{" "}
                  {user.realtor.virtualPropertyTour ? "Yes" : "No"}
                </p>
                <p>
                  <strong>Years of Experience:</strong>{" "}
                  {user.realtor.yearsOfExperience}
                </p>
              </>
            ) : user.carDealership ? (
              <>
                <p>
                  <strong>Business Name:</strong>{" "}
                  {user.carDealership.businessName}
                </p>
                <p>
                  <strong>Showroom Locations:</strong>{" "}
                  {user.carDealership.showroomLocations}
                </p>
                <p>
                  <strong>Test Drive Policy:</strong>{" "}
                  {user.carDealership.testDrivePolicy}
                </p>
                <p>
                  <strong>Financing Options:</strong>{" "}
                  {(() => {
                    try {
                      const options = JSON.parse(
                        user.carDealership.financingOptions
                      );
                      return `In House Financing: ${
                        options.inHouseFinancing ? "Yes" : "No"
                      }, Third Party Banks: ${
                        options.thirdPartyBanks ? "Yes" : "No"
                      }, Lease Options: ${options.leaseOptions ? "Yes" : "No"}`;
                    } catch (error) {
                      return user.carDealership.financingOptions;
                    }
                  })()}
                </p>
                <p>
                  <strong>Trade In Available:</strong>{" "}
                  {user.carDealership.tradeInAvailable ? "Yes" : "No"}
                </p>
                <p>
                  <strong>Service Warranty Info:</strong>{" "}
                  {user.carDealership.serviceWarrantyInfo}
                </p>
                <p>
                  <strong>Business Registration:</strong>{" "}
                  {user.carDealership.businessRegistration}
                </p>
                <p>
                  <strong>Years in Business:</strong>{" "}
                  {user.carDealership.yearsInBusiness}
                </p>
              </>
            ) : user.immigrationConsultant ? (
              <>
                <p>
                  <strong>Business Name:</strong>{" "}
                  {user.immigrationConsultant.businessName}
                </p>
                <p>
                  <strong>Business Address:</strong>{" "}
                  {user.immigrationConsultant.businessAddress}
                </p>
                <p>
                  <strong>License Number:</strong>{" "}
                  {user.immigrationConsultant.licenseNumber}
                </p>
                <p>
                  <strong>Countries Served:</strong>{" "}
                  {user.immigrationConsultant.countriesServed}
                </p>
                <p>
                  <strong>Consultation Fee:</strong>{" "}
                  {user.immigrationConsultant.consultationFee}
                </p>
                <p>
                  <strong>Business Registration:</strong>{" "}
                  {user.immigrationConsultant.businessRegistration}
                </p>
                <p>
                  <strong>Partnered Legal Firms:</strong>{" "}
                  {user.immigrationConsultant.partneredLegalFirms || "N/A"}
                </p>
                <p>
                  <strong>Website/Social Media:</strong>{" "}
                  {user.immigrationConsultant.websiteOrSocialMedia ? (
                    <a
                      href={user.immigrationConsultant.websiteOrSocialMedia}
                      target="_blank"
                      rel="noopener noreferrer"
                      className="text-blue-600 underline"
                    >
                      {user.immigrationConsultant.websiteOrSocialMedia}
                    </a>
                  ) : (
                    "N/A"
                  )}
                </p>
                <p>
                  <strong>Years of Experience:</strong>{" "}
                  {user.immigrationConsultant.yearsOfExperience}
                </p>
                <p>
                  <strong>Services Offered:</strong>{" "}
                  {user.immigrationConsultant.servicesOffered}
                </p>
                <p>
                  <strong>Languages Spoken:</strong>{" "}
                  {user.immigrationConsultant.languagesSpoken}
                </p>
              </>
            ) : (
              <p>No business details available.</p>
            )}
          </div>
          {/* Right: Business Info PDF */}
          {renderPDFViewer("Business Info Document")}
        </div>
      );
    } else if (step === 3) {
      return (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {/* Left: License Details */}
          <div className="p-5 border rounded shadow-sm">
            <h2 className="text-2xl font-bold mb-4">License Details</h2>
            {user.realtor ? (
              <p>
                <strong>License Number:</strong>{" "}
                {user.realtor.realEstateLicenseNumber}
              </p>
            ) : user.carDealership ? (
              <p>
                <strong>Dealership License Number:</strong>{" "}
                {user.carDealership.dealershipLicenseNumber}
              </p>
            ) : user.immigrationConsultant ? (
              <p>
                <strong>License Number:</strong>{" "}
                {user.immigrationConsultant.licenseNumber}
              </p>
            ) : (
              <p>No license details available.</p>
            )}
          </div>
          {/* Right: License Document PDF */}
          {renderPDFViewer("License Document")}
        </div>
      );
    }
  };

  return (
    <div className="min-h-screen p-5">
      {/* Back to Users Button */}
      <button
        onClick={handleBack}
        className="px-4 py-2 rounded hover:bg-gray-200 transition mb-5"
      >
        ← Back to Users
      </button>

      {/* Step Navigation */}
      <div className="flex justify-between mb-4">
        <button
          onClick={() => setStep((prev) => Math.max(prev - 1, 1))}
          disabled={step === 1}
          className={`px-4 py-2 rounded ${
            step === 1
              ? "bg-gray-300"
              : "bg-blue-600 text-white hover:bg-blue-700"
          }`}
        >
          ← Previous
        </button>
        <span className="text-lg font-semibold">
          {step === 1
            ? "User Details"
            : step === 2
            ? "Business Details"
            : "License Details"}
        </span>
        <button
          disabled={step === 3 && user?.userVerified === true}
          onClick={() =>
            step === 3 ? setShowModal(true) : setStep((prev) => prev + 1)
          }
          className={`px-4 py-2 rounded ${
            step === 3 && user?.userVerified === true
              ? "bg-gray-400 cursor-not-allowed"
              : "bg-blue-600 text-white hover:bg-blue-700"
          }`}
        >
          {step === 3 ? "Verify User" : "Next →"}
        </button>
      </div>

      {/* Step Content */}
      {renderStepContent()}

      {/* Modal Confirmation */}
      {showModal && (
        <div className="fixed inset-0 bg-gray-700 bg-opacity-50 flex justify-center items-center">
          <div className="bg-white p-6 rounded">
            <h2 className="text-xl font-bold mb-4">Confirm Verification</h2>
            <p>Are you sure you want to verify this user?</p>
            <div className="mt-4 flex justify-end space-x-2">
              <button
                onClick={() => setShowModal(false)}
                className="px-4 py-2 bg-gray-300 rounded"
              >
                Cancel
              </button>
              <button
                onClick={() => handleVerifyUser(user.id)}
                className="px-4 py-2 bg-blue-600 text-white rounded"
              >
                Verify
              </button>
            </div>
          </div>
        </div>
      )}
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/car-dealer/add-listing/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { useState } from "react";
import { useRouter } from "next/navigation";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";

const AddCarListing = () => {
  const [formData, setFormData] = useState({
    model: "",
    make: "",
    price: "",
    year: "",
    mileage: "",
    exteriorColor: "",
    interiorColor: "",
    transmission: "",
    fuelType: "",
    vin: "",
    vehicleType: "",
    noOfSeats: "",
    status: "",
  });

  const [images, setImages] = useState<File[]>([]);
  const [errorMessage, setErrorMessage] = useState("");
  const [successMessage, setSuccessMessage] = useState("");
  const router = useRouter();
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Handle input changes for text/number fields
  const handleChange = (
    e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>
  ) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  // Handle image uploads
  const handleFileChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    if (e.target.files) {
      setImages(Array.from(e.target.files));
    }
  };

  // Basic validation for required fields and image count
  const validateForm = () => {
    // Check that every field is provided (adjust as needed)
    for (const [key, value] of Object.entries(formData)) {
      if (!value) {
        setErrorMessage(`Field "${key}" is required.`);
        return false;
      }
    }

    if (isNaN(Number(formData.price)) || Number(formData.price) <= 0) {
      setErrorMessage("Please enter a valid price.");
      return false;
    }

    if (images.length === 0 || images.length > 3) {
      setErrorMessage("You must upload between 1 and 3 images.");
      return false;
    }

    setErrorMessage(""); // Clear any previous error
    return true;
  };

  // Submit form data
  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();

    if (!validateForm()) {
      return;
    }

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataObj = new FormData();
      // Append every field from the formData state
      Object.entries(formData).forEach(([key, value]) => {
        formDataObj.append(key, value);
      });
      // Append images
      images.forEach((image) => formDataObj.append("images", image));

      const response = await fetch(
        `${endpoint}api/protected/car-listing/add-car-listing`,
        {
          method: "POST",
          headers: {
            Authorization: `Bearer ${token}`,
          },
          body: formDataObj,
        }
      );

      if (response.ok) {
        setSuccessMessage("Car listing created successfully!");
        setErrorMessage("");
        router.push("/dashboard/car-dealer/car-listings");
      } else {
        setErrorMessage("Failed to create car listing. Please try again.");
        setSuccessMessage("");
      }
    } catch (error) {
      setErrorMessage("An error occurred. Please try again.");
      setSuccessMessage("");
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 ">
      {/* Back Button */}
      <Link href="/dashboard/car-dealer">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>
      <div className="max-w-4xl mx-auto p-6 shadow-lg rounded-lg mt-8">
        <h1 className="text-2xl font-bold mb-6">Add Car Listing</h1>
        <form onSubmit={handleSubmit}>
          {/* Model */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Model</label>
            <input
              type="text"
              name="model"
              value={formData.model}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Make */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Make</label>
            <input
              type="text"
              name="make"
              value={formData.make}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Price */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Price</label>
            <input
              type="number"
              name="price"
              value={formData.price}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Year */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Year</label>
            <input
              type="number"
              name="year"
              value={formData.year}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Mileage */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Mileage</label>
            <input
              type="number"
              name="mileage"
              value={formData.mileage}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Exterior Color */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Exterior Color</label>
            <input
              type="text"
              name="exteriorColor"
              value={formData.exteriorColor}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Interior Color */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Interior Color</label>
            <input
              type="text"
              name="interiorColor"
              value={formData.interiorColor}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Transmission */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Transmission</label>
            <input
              type="text"
              name="transmission"
              value={formData.transmission}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Fuel Type */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Fuel Type</label>
            <input
              type="text"
              name="fuelType"
              value={formData.fuelType}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* VIN */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">VIN</label>
            <input
              type="text"
              name="vin"
              value={formData.vin}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Vehicle Type */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Vehicle Type</label>
            <input
              type="text"
              name="vehicleType"
              value={formData.vehicleType}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Number of Seats */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Number of Seats</label>
            <input
              type="number"
              name="noOfSeats"
              value={formData.noOfSeats}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Status */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">Status</label>
            <input
              type="text"
              name="status"
              value={formData.status}
              onChange={handleChange}
              className="w-full border rounded p-2"
              required
            />
          </div>

          {/* Image Upload */}
          <div className="mb-4">
            <label className="block font-semibold mb-2">
              Upload Images (Max: 3)
            </label>
            <input
              type="file"
              multiple
              accept="image/*"
              onChange={handleFileChange}
              className="w-full border rounded p-2"
            />
          </div>

          {errorMessage && <p className="text-red-500">{errorMessage}</p>}
          {successMessage && <p className="text-blue-500">{successMessage}</p>}

          {/* Submit Button */}
          <Button
            type="submit"
            className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-500 mt-3"
          >
            Submit Car Listing
          </Button>
        </form>
      </div>
    </div>
  );
};

export default AddCarListing;
````

## File: Frontend/src/app/dashboard/car-dealer/availability/page.tsx
````typescript
"use client";
import Availability from "@/components/availability/AvailabilityPage";
import SideCard from "@/components/Sidecard";


const services = ["Dashboard", "Listings","Availability", "Bookings"];
  const urls = ["/dashboard/car-dealer", "/dashboard/car-dealer/car-listings/", "/dashboard/car-dealer/availability/", "/dashboard/car-dealer/bookings/"];


const RealtorAvailability = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <Availability />
      </div>
    </div>
  );
};

export default RealtorAvailability;
````

## File: Frontend/src/app/dashboard/car-dealer/bookings/page.tsx
````typescript
"use client";
import BookingTable from "@/components/availability/BookingTable";
import SideCard from "@/components/Sidecard";

const services = ["Dashboard", "Listings","Availability", "Bookings"];
  const urls = ["/dashboard/car-dealer", "/dashboard/car-dealer/car-listings/", "/dashboard/car-dealer/availability/", "/dashboard/car-dealer/bookings/"];


const CarBooking = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <BookingTable />
      </div>
    </div>
  );
};

export default CarBooking;
````

## File: Frontend/src/app/dashboard/car-dealer/car-listings/[id]/page.tsx
````typescript
"use client";

import { useParams, useRouter } from "next/navigation";
import { useEffect, useState } from "react";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import {
  FiEdit,
  FiTrash2,
  FiArrowLeft,
  FiCalendar,
  FiDroplet,
  FiSettings,
  FiUsers,
  FiPhoneCall,
  FiMail,
  FiMapPin,
  FiDollarSign,
} from "react-icons/fi";
import { MdSpeed, MdCarRental, MdFormatPaint } from "react-icons/md";
import { Swiper, SwiperSlide } from "swiper/react";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";
import { Card, CardContent } from "@/components/ui/card";

const ViewCarListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [listing, setListing] = useState<any>(null);
  const [userRole, setUserRole] = useState<string | null>(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);

  useEffect(() => {
    if (id) {
      const fetchListing = async () => {
        try {
          const endpoint = process.env.NEXT_PUBLIC_API_URL;
          // Fetch token
          const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
          const tokenData = await tokenResponse.json();
          const token = tokenData?.token;
          const role = tokenData?.role;
          if (!token) {
            throw new Error("Invalid authentication token");
          }
          setUserRole(role);

          // Fetch car listing
          const response = await fetch(
            `${endpoint}api/protected/car-listing/carlisting/${id}`,
            {
              headers: { Authorization: `Bearer ${token}` },
            }
          );
          if (!response.ok) {
            throw new Error("Failed to fetch car listing");
          }
          const data = await response.json();
          setListing(data);
        } catch (err: any) {
          setError(err.message);
        } finally {
          setLoading(false);
        }
      };
      fetchListing();
    }
  }, [id]);

  const handleDelete = async () => {
    if (confirm("Are you sure you want to delete this car listing?")) {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) {
          throw new Error("Invalid authentication token");
        }
        const response = await fetch(
          `${endpoint}api/protected/car-listing/delete-car-listing/${id}`,
          {
            method: "DELETE",
            headers: { Authorization: `Bearer ${token}` },
          }
        );
        if (!response.ok) {
          throw new Error("Failed to delete car listing");
        }
        alert("Car listing deleted successfully");
        router.push("/dashboard/car-dealer/car-listings");
      } catch (err: any) {
        alert(`Error deleting car listing: ${err.message}`);
      }
    }
  };

  // Helper functions to format dealership info
  const formatFinancingOptions = (optionsStr: string) => {
    return optionsStr
      .replace(/[{}"]/g, "")
      .split(",")
      .map((o) => o.trim());
  };

  const formatShowroomLocations = (locationsStr: string) => {
    return locationsStr.replace(/[{}"]/g, "");
  };

  if (loading) {
    return <p className="text-center text-lg text-gray-500">Loading...</p>;
  }
  if (error) {
    return <p className="text-center text-red-500 text-lg">Error: {error}</p>;
  }
  if (!listing) {
    return (
      <p className="text-center text-gray-500 text-lg">No car listing found</p>
    );
  }

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      <Link href="/dashboard/car-dealer/car-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>

      <div className="flex flex-col md:flex-row gap-6">
        {/* Main Listing Card */}
        <div className="md:w-2/3">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              {/* Image Carousel */}
              {listing.carImages && listing.carImages.length > 0 && (
                <Swiper
                  navigation={true}
                  modules={[Navigation]}
                  className="w-full h-96 rounded-lg shadow-lg mb-6"
                >
                  {listing.carImages.map((image, index) => (
                    <SwiperSlide key={index}>
                      <img
                        src={image.base64}
                        alt={`Car Image ${index + 1}`}
                        className="w-full h-96 object-cover rounded-lg"
                      />
                    </SwiperSlide>
                  ))}
                </Swiper>
              )}
              {/* Car Details */}
              <div className="mb-4">
                <h1 className="text-3xl font-semibold">
                  {listing.model} - {listing.make}
                </h1>
                {listing.createdAt && (
                  <p className="mt-2 text-sm text-gray-500">
                    Created At:{" "}
                    {new Date(listing.createdAt).toLocaleDateString()}
                  </p>
                )}
                <p className="text-2xl mt-2 text-blue-600 font-bold flex items-center gap-1">
                  <FiDollarSign size={24} />
                  {listing.price ?? "N/A"}
                </p>
              </div>
              {/* Specifications */}
              <div className="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-3 gap-4">
                <div className="flex items-center gap-1">
                  <FiCalendar size={20} />
                  <p className="text-lg font-semibold">
                    {listing.year ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <MdSpeed size={20} />
                  <p className="text-lg font-semibold">
                    {listing.mileage ? `${listing.mileage} km` : "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiSettings size={20} />
                  <p className="text-lg font-semibold">
                    {listing.transmission ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiDroplet size={20} />
                  <p className="text-lg font-semibold">
                    {listing.fuelType ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiUsers size={20} />
                  <p className="text-lg font-semibold">
                    {listing.noOfSeats ? `${listing.noOfSeats} Seats` : "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <MdFormatPaint size={20} />
                  <p className="text-lg font-semibold">
                    {listing.exteriorColor ?? "N/A"}
                  </p>
                </div>
              </div>

              {/* Action Buttons */}
              <div className="mt-6 flex flex-wrap gap-4">
                <Link href={`/dashboard/car-dealer/edit-listing/${id}`}>
                  <Button variant="default" className="flex items-center gap-2">
                    <FiEdit size={18} />
                    Edit Listing
                  </Button>
                </Link>
                <Button
                  onClick={handleDelete}
                  variant="destructive"
                  className="flex items-center gap-2"
                >
                  <FiTrash2 size={18} />
                  Delete Listing
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>

        {/* Separate Dealership Info Container */}
        {listing.dealership && (
          <div className="md:w-1/3">
            <Card className="shadow-lg">
              <CardContent className="p-6">
                <h2 className="text-xl font-bold mb-4">Contact Details: </h2>
                <div className="mb-3">
                  <p className="font-semibold">{listing.dealership.fullName}</p>
                </div>
                <div className="flex items-center mb-3">
                  <FiPhoneCall size={18} className="text-blue-500 mr-2" />
                  <p>{listing.dealership.phoneNo}</p>
                </div>
                <div className="flex items-center mb-3">
                  <FiMail size={18} className="text-blue-500 mr-2" />
                  <p>{listing.dealership.email}</p>
                </div>
                {listing.dealership.carDealership && (
                  <>
                    <div className="flex items-center mb-3">
                      <FiMapPin size={18} className="text-red-500 mr-2" />
                      <div>
                        <p className="text-lg">
                          {listing.dealership.carDealership.businessName}
                        </p>
                        <p className="text-lg">
                          {formatShowroomLocations(
                            listing.dealership.carDealership.showroomLocations
                          )}
                        </p>
                      </div>
                    </div>
                    <div className="mb-3">
                      <ul className="list-disc list-inside list-none">
                        {formatFinancingOptions(
                          listing.dealership.carDealership.financingOptions
                        ).map((option, idx) => (
                          <li key={idx} className="text-lg">
                            {option === "inHouseFinancing:true" &&
                              "🏠 In-House Financing"}
                            {option === "thirdPartyBanks:true" &&
                              "🏦 Third-Party Banks"}
                            {option === "leaseOptions:true" &&
                              "📄 Lease Options"}
                            {option === "inHouseFinancing:false" &&
                              "❌ No In-House Financing"}
                            {option === "thirdPartyBanks:false" &&
                              "❌ No Third-Party Banks"}
                            {option === "leaseOptions:false" &&
                              "❌ No Lease Options"}
                          </li>
                        ))}
                      </ul>
                    </div>
                  </>
                )}
              </CardContent>
            </Card>
          </div>
        )}
      </div>
    </div>
  );
};

export default ViewCarListing;
````

## File: Frontend/src/app/dashboard/car-dealer/car-listings/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Listings",
  "Availability",
  "Bookings",
  "Profile",
];
const urls = [
  "/dashboard/car-dealer",
  "/dashboard/car-dealer/car-listings/",
  "/dashboard/car-dealer/availability/",
  "/dashboard/car-dealer/bookings/",
  "/dashboard/car-dealer/profile",
];

const CarsListing = () => {
  const [carListings, setCarListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);
  const [refresh, setRefresh] = useState(false);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const carResponse = await fetch(
          `${endpoint}api/protected/car-listing/by-id-car-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!carResponse.ok) throw new Error("Failed to fetch car listings");

        const carData = await carResponse.json();
        setCarListings(carData);
        setFilteredListings(carData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);
  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = carListings.filter((car) => {
      return (
        (!filters.make ||
          car.make?.toLowerCase().includes(filters.make.toLowerCase())) &&
        (!filters.model ||
          car.model?.toLowerCase().includes(filters.model.toLowerCase())) &&
        (!filters.price || car.price <= parseFloat(filters.price))
      );
    });

    setFilteredListings(filtered.slice());
  };

  // Debugging UI Update
  useEffect(() => {}, [filteredListings]);

  const carFiltersConfig = [
    { name: "make", type: "text", placeholder: "Make (e.g. Toyota)" },
    { name: "model", type: "text", placeholder: "Model (e.g. Corolla)" },
    { name: "price", type: "number", placeholder: "Max Price" },
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Links" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Cars Listing</h2>
          <ReusableFilter
            filtersConfig={carFiltersConfig}
            onFilterChange={handleFilterChange}
          />
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && filteredListings.length > 0 ? (
          <Listings key={refresh} listings={filteredListings} />
        ) : (
          <p>No cars found.</p>
        )}
      </div>
    </div>
  );
};

export default CarsListing;
````

## File: Frontend/src/app/dashboard/car-dealer/edit-listing/[id]/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { useEffect, useState } from "react";
import { useRouter, useParams } from "next/navigation";
import { Card } from "@/components/ui/card";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";

const EditCarListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [formData, setFormData] = useState({
    model: "",
    make: "",
    price: "",
    year: "",
    mileage: "",
    exteriorColor: "",
    interiorColor: "",
    transmission: "",
    fuelType: "",
    vin: "",
    vehicleType: "",
    noOfSeats: "",
    status: "",
  });

  // existingImages will contain both server images (as base64) and previews for newly added images.
  const [existingImages, setExistingImages] = useState([]);
  // newImages holds only new File objects
  const [newImages, setNewImages] = useState([]);
  const [errorMessage, setErrorMessage] = useState("");
  const [successMessage, setSuccessMessage] = useState("");

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Helper function to convert a base64 data URL to a File object.
  const dataURLtoFile = (dataurl, filename) => {
    const arr = dataurl.split(",");
    const mimeMatch = arr[0].match(/:(.*?);/);
    if (!mimeMatch) return null;
    const mime = mimeMatch[1];
    const bstr = atob(arr[1]);
    let n = bstr.length;
    const u8arr = new Uint8Array(n);
    while (n--) {
      u8arr[n] = bstr.charCodeAt(n);
    }
    return new File([u8arr], filename, { type: mime });
  };

  useEffect(() => {
    const fetchData = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const response = await fetch(
          `${endpoint}api/protected/car-listing/carlisting/${id}`,
          { headers: { Authorization: `Bearer ${token}` } }
        );

        if (!response.ok) throw new Error("Failed to fetch listing data");

        const data = await response.json();
        setFormData({
          model: data.model ?? "",
          make: data.make ?? "",
          price: data.price?.toString() ?? "",
          year: data.year?.toString() ?? "",
          mileage: data.mileage?.toString() ?? "",
          exteriorColor: data.exteriorColor ?? "",
          interiorColor: data.interiorColor ?? "",
          transmission: data.transmission ?? "",
          fuelType: data.fuelType ?? "",
          vin: data.vin ?? "",
          vehicleType: data.vehicleType ?? "",
          noOfSeats: data.noOfSeats?.toString() ?? "",
          status: data.status ?? "",
        });
        // Set existing images from the server as base64 strings.
        setExistingImages(data.carImages.map((img) => img.base64));
      } catch (error) {
        setErrorMessage("Failed to fetch listing data: " + error.message);
      }
    };
    fetchData();
  }, [id, endpoint]);

  const handleChange = (e) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  const handleFileChange = (e) => {
    if (e.target.files) {
      const filesArray = Array.from(e.target.files);
      const newPreviews = filesArray.map((file) => URL.createObjectURL(file));
      setNewImages((prev) => [...prev, ...filesArray]);
      setExistingImages((prev) => [...prev, ...newPreviews]);
    }
  };

  const removeImage = (index) => {
    const newExisting = [...existingImages];
    newExisting.splice(index, 1);
    setExistingImages(newExisting);
    // Determine if the removed image is from newImages.
    if (index >= existingImages.length - newImages.length) {
      const newIndex = index - (existingImages.length - newImages.length);
      const newFiles = [...newImages];
      newFiles.splice(newIndex, 1);
      setNewImages(newFiles);
    }
  };

  const handleSubmit = async (e) => {
    e.preventDefault();
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;
      const formDataObj = new FormData();

      Object.keys(formData).forEach((key) => {
        formDataObj.append(key, formData[key]);
      });

      // Calculate how many images came from the server.
      const serverImagesCount = existingImages.length - newImages.length;
      const serverImages = existingImages.slice(0, serverImagesCount);

      // Convert each server image (base64 string) to a File and append.
      serverImages.forEach((dataURL, index) => {
        const file = dataURLtoFile(dataURL, `server-image-${index}.png`);
        if (file) {
          formDataObj.append("images", file);
        }
      });

      // Append new images (already File objects).
      newImages.forEach((image) => {
        formDataObj.append("images", image);
      });

      const response = await fetch(
        `${endpoint}api/protected/car-listing/update-car-listing/${id}`,
        {
          method: "PUT",
          headers: { Authorization: `Bearer ${token}` },
          body: formDataObj,
        }
      );

      if (!response.ok)
        throw new Error(`Failed to update listing: ${response.statusText}`);

      setSuccessMessage("Car listing updated successfully!");
      router.push(`/dashboard/car-dealer/car-listings/${id}`);
    } catch (error) {
      setErrorMessage("Error updating listing: " + error.message);
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      {/* Back Button */}
      <Link href="/dashboard/car-dealer/car-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>
      <Card className="shadow-lg p-6">
        <h1 className="text-2xl font-bold mb-6">Edit Car Listing</h1>
        <form onSubmit={handleSubmit}>
          {Object.keys(formData).map(
            (key) =>
              // Exclude fields not intended for editing
              !["id", "dealership", "createdAt", "carImages"].includes(key) && (
                <div key={key} className="mb-4">
                  <label className="block font-semibold mb-2 capitalize">
                    {key.replace(/([A-Z])/g, " $1")}
                  </label>
                  <input
                    type="text"
                    name={key}
                    value={formData[key as keyof typeof formData]}
                    onChange={handleChange}
                    className="w-full border rounded p-2"
                  />
                </div>
              )
          )}

          <div className="mb-4">
            <label className="block font-semibold mb-2">Add Images</label>
            <input
              type="file"
              multiple
              accept="image/*"
              onChange={handleFileChange}
              className="w-full border rounded p-2"
            />
            <div className="flex flex-wrap gap-4 mt-4">
              {existingImages.map((image, index) => (
                <div key={index} className="relative">
                  <img
                    src={image}
                    alt={`Car Image ${index}`}
                    className="w-24 h-24 object-cover rounded"
                  />
                  <button
                    type="button"
                    className="absolute top-0 right-0 bg-red-500 text-white p-1 rounded"
                    onClick={() => removeImage(index)}
                  >
                    &times;
                  </button>
                </div>
              ))}
            </div>
          </div>

          <Button
            type="submit"
            className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-500 mt-3"
          >
            Update Listing
          </Button>
        </form>
        {errorMessage && <p className="text-red-500">{errorMessage}</p>}
        {successMessage && <p className="text-blue-500">{successMessage}</p>}
      </Card>
    </div>
  );
};

export default EditCarListing;
````

## File: Frontend/src/app/dashboard/car-dealer/page.tsx
````typescript
"use client";

import QuickLinks from "@/components/QuickLinks";
import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import { useEffect, useState } from "react";

export default function DashboardLayout() {
  const [listings, setListings] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  const services = ["Dashboard", "Listings","Availability", "Bookings"];
  const urls = ["/dashboard/car-dealer", "/dashboard/car-dealer/car-listings/", "/dashboard/car-dealer/availability/", "/dashboard/car-dealer/bookings/"];

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        // Fetch token
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });

        if (!tokenResponse.ok) {
          throw new Error("Failed to get authentication token");
        }

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;

        if (!token) {
          throw new Error("Invalid authentication token");
        }

        // Fetch car listings
        const response = await fetch(
          `${endpoint}api/protected/car-listing/by-id-car-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (response.status === 404) {
          throw new Error("No listing found");
        }
        

        const data = await response.json();
        setListings(data);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Links" urls={urls}/>
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Car Dealer Dashboard</h2>
          <QuickLinks links={[
            { label: "Add Listing", href: "car-dealer/add-listing" },
            { label: "View Listings", href: "car-dealer/car-listings" },
            { label: "Requests", href: "car-dealer/availability" },
          ]} />
          <h2 className="text-2xl font-bold mb-6 mt-5">View added listings</h2>
          {loading && <p>Loading...</p>}
          {error && <p>Error: {error}</p>}
          {!loading && !error && listings && <Listings listings={listings} />}
        </div>
      </div>
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/consultant/availability/page.tsx
````typescript
"use client";
import Availability from "@/components/availability/AvailabilityPage";
import SideCard from "@/components/Sidecard";



const services = ["Dashboard", "Availability", "Bookings"];
const urls = ["/dashboard/consultant", "/dashboard/consultant/availability", "/dashboard/consultant/bookings/"];



const ICAvailability = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <Availability />
      </div>
    </div>
  );
};

export default ICAvailability;
````

## File: Frontend/src/app/dashboard/consultant/bookings/page.tsx
````typescript
"use client";
import BookingTable from "@/components/availability/BookingTable";
import SideCard from "@/components/Sidecard";


const services = ["Dashboard", "Availability", "Bookings"];
const urls = ["/dashboard/consultant", "/dashboard/consultant/availability", "/dashboard/consultant/bookings/"];



const ICBooking = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <BookingTable />
      </div>
    </div>
  );
};

export default ICBooking;
````

## File: Frontend/src/app/dashboard/consultant/page.tsx
````typescript
"use client";

import QuickLinks from "@/components/QuickLinks";
import SideCard from "@/components/Sidecard";
import UpcomingConsultantMeetings from "@/components/consultant/UpcomingMeetings";
// import { useEffect, useState } from "react";

export default function DashboardLayout() {

  const services = ["Dashboard", "Availability", "Bookings"];
  const urls = ["/dashboard/consultant", "/dashboard/consultant/availability", "/dashboard/consultant/bookings/"];

 
  //   const fetchListings = async () => {
  //     try {
  //       const endpoint = process.env.NEXT_PUBLIC_API_URL;

  //       // Fetch token
  //       const tokenResponse = await fetch(`${endpoint}auth/token`, {
  //         credentials: "include",
  //       });

  //       if (!tokenResponse.ok) {
  //         throw new Error("Failed to get authentication token");
  //       }

  //       const tokenData = await tokenResponse.json();
  //       const token = tokenData?.token;

  //       if (!token) {
  //         throw new Error("Invalid authentication token");
  //       }

  //       // Fetch car listings
  //       const response = await fetch(
  //         `${endpoint}api/protected/`,
  //         {
  //           headers: { Authorization: `Bearer ${token}` },
  //         }
  //       );

  //       if (response.status === 404) {
  //         throw new Error("No listing found");
  //       }
        

  //       const data = await response.json();
  //       setListings(data);
  //     } catch (err) {
  //       setError(err.message);
  //     } finally {
  //       setLoading(false);
  //     }
  //   };

  //   fetchListings();
  // }, []);

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Links" urls={urls}/>
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Immigration Consultant Dashboard</h2>
          <QuickLinks links={[
            { label: "Add Availability", href: "/dashboard/consultant/availability" },
            { label: "View Bookings", href: "/dashboard/consultant/bookings" },
          ]} />
          <h2 className="text-2xl font-bold mb-6 mt-5">Upcoming Meetings</h2>
          {/* {loading && <p>Loading...</p>}
          {error && <p>Error: {error}</p>}
          {!loading && !error && listings && <Listings listings={listings} />} */}
          <UpcomingConsultantMeetings/>
        </div>
      </div>
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/layout.tsx
````typescript
import Header from "@/components/Header";
import { redirect } from "next/navigation";
import { getSession } from "@/lib/auth";
import React, { ReactNode } from "react";

async function Layout({ children }: { children: ReactNode }) {
  const session = await getSession();

  if (!session) {
    redirect("/");
  }

  return (
    <div className="flex flex-col h-screen min-w-full bg-background">
      <Header />
      <main className="w-full h-full">{children}</main>
    </div>
  );
}

export default Layout;
````

## File: Frontend/src/app/dashboard/not-verified/page.tsx
````typescript
"use client";
import { useSearchParams, useRouter } from "next/navigation";
import { FaCheckCircle } from "react-icons/fa";

export default function NotVerified() {
  const searchParams = useSearchParams();
  const reason = searchParams.get("reason");
  let message = "";
  if (reason === "user") {
    message = "Your account verification is pending.";
  }
  return (
    <div className="flex flex-col items-center justify-center p-6">
      <div className="shadow-lg rounded-2xl p-8 text-center max-w-md w-full">
        <FaCheckCircle className="text-blue-500 w-16 h-16 mx-auto" />
        <h1 className="text-2xl font-semibold mt-4">
          Form Submitted Successfully!
        </h1>
        <p className="text-gray-600 mt-2">{`${message} We will notify you once the process is complete.`}</p>
      </div>
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/page.tsx
````typescript
import React from "react";

const Dashboard = () => {
  return <div>Dashboard</div>;
};

export default Dashboard;
````

## File: Frontend/src/app/dashboard/realtor/add-listing/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { useState } from "react";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";

const AddListing = () => {
  const [formData, setFormData] = useState({
    title: "",
    description: "",
    price: "",
    location: "",
    bedrooms: "",
    bathrooms: "",
    squareFeet: "",
    openhouse: false,
    startDate: "",
    endDate: "",
    startTime: "",
    endTime: "",
  });

  const [images, setImages] = useState<File[]>([]);
  const [errorMessage, setErrorMessage] = useState("");
  const [successMessage, setSuccessMessage] = useState("");

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Handle input changes
  const handleChange = (
    e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>
  ) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  // Toggle open house checkbox
  const handleToggleOpenHouse = () => {
    setFormData((prev) => ({ ...prev, openhouse: !prev.openhouse }));
  };

  // Handle image uploads
  const handleFileChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    if (e.target.files) {
      setImages(Array.from(e.target.files));
    }
  };

  // Validation function
  const validateForm = () => {
    if (!formData.title || !formData.price || !formData.location) {
      setErrorMessage("Title, price, and location are required.");
      return false;
    }

    if (isNaN(Number(formData.price)) || Number(formData.price) <= 0) {
      setErrorMessage("Please enter a valid price.");
      return false;
    }

    if (formData.openhouse) {
      if (
        !formData.startDate ||
        !formData.endDate ||
        !formData.startTime ||
        !formData.endTime
      ) {
        setErrorMessage(
          "Start and end date, and time are required for open house."
        );
        return false;
      }
      if (new Date(formData.startDate) > new Date(formData.endDate)) {
        setErrorMessage("Start date must be earlier than end date.");
        return false;
      }
    }

    if (images.length === 0 || images.length > 3) {
      setErrorMessage("You must upload between 1 and 3 images.");
      return false;
    }

    setErrorMessage(""); // Clear any previous error message
    return true;
  };

  // Submit form
  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();

    if (!validateForm()) {
      return;
    }

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const formDataObj = new FormData();
      Object.entries(formData).forEach(([key, value]) => {
        formDataObj.append(key, value);
      });

      images.forEach((image) => formDataObj.append("images", image));

      const response = await fetch(
        `${endpoint}api/protected/house-listing/add-house-listing`,
        {
          method: "POST",
          headers: {
            Authorization: `Bearer ${token}`,
          },
          body: formDataObj,
        }
      );

      if (response.ok) {
        setSuccessMessage("Listing created successfully!");
        setErrorMessage("");
      } else {
        setErrorMessage("Failed to create listing. Please try again.");
        setSuccessMessage("");
      }
    } catch (error) {
      setErrorMessage("An error occurred. Please try again.");
      setSuccessMessage("");
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-2">
      {/* Back Button */}
      <Link href="/dashboard/realtor/house-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>
      <div className="max-w-4xl mx-auto p-6 bg-white shadow-lg rounded-lg mt-8">
        <h1 className="text-2xl font-bold mb-6">Add House Listing</h1>
        <form onSubmit={handleSubmit}>
          {/* Title */}
          <input
            type="text"
            name="title"
            value={formData.title}
            onChange={handleChange}
            className="w-full border rounded p-2 mb-4"
            placeholder="Title"
            required
          />

          {/* Description */}
          <textarea
            name="description"
            value={formData.description}
            onChange={handleChange}
            className="w-full border rounded p-2 mb-4"
            placeholder="Description"
          />

          {/* Price & Location */}
          <div className="grid grid-cols-2 gap-4 mb-4">
            <input
              type="number"
              name="price"
              value={formData.price}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Price"
              required
            />
            <input
              type="text"
              name="location"
              value={formData.location}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Location"
              required
            />
          </div>

          {/* Bedrooms, Bathrooms, Square Feet */}
          <div className="grid grid-cols-3 gap-4 mb-4">
            <input
              type="number"
              name="bedrooms"
              value={formData.bedrooms}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Bedrooms"
            />
            <input
              type="number"
              name="bathrooms"
              value={formData.bathrooms}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Bathrooms"
            />
            <input
              type="number"
              name="squareFeet"
              value={formData.squareFeet}
              onChange={handleChange}
              className="w-full border rounded p-2"
              placeholder="Square Feet"
            />
          </div>

          {/* Open House Checkbox */}
          <label className="flex items-center space-x-2 mb-4">
            <input
              type="checkbox"
              checked={formData.openhouse}
              onChange={handleToggleOpenHouse}
            />
            <span>Open House</span>
          </label>

          {/* Open House Details */}
          {formData.openhouse && (
            <div className="grid grid-cols-2 gap-4">
              <input
                type="date"
                name="startDate"
                value={formData.startDate}
                onChange={handleChange}
                className="w-full border rounded p-2"
              />
              <input
                type="date"
                name="endDate"
                value={formData.endDate}
                onChange={handleChange}
                className="w-full border rounded p-2"
              />
              <input
                type="time"
                name="startTime"
                value={formData.startTime}
                onChange={handleChange}
                className="w-full border rounded p-2"
              />
              <input
                type="time"
                name="endTime"
                value={formData.endTime}
                onChange={handleChange}
                className="w-full border rounded p-2"
              />
            </div>
          )}

          {/* Image Upload */}
          <input
            type="file"
            multiple
            accept="image/*"
            onChange={handleFileChange}
            className="w-full border rounded p-2 mb-4"
          />

          {errorMessage && <p className="text-red-500">{errorMessage}</p>}
          {successMessage && <p className="text-blue-500">{successMessage}</p>}

          {/* Submit Button */}
          <Button
            type="submit"
            className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-500"
          >
            Submit Listing
          </Button>
        </form>
      </div>
    </div>
  );
};

export default AddListing;
````

## File: Frontend/src/app/dashboard/realtor/availability/page.tsx
````typescript
"use client";
import Availability from "@/components/availability/AvailabilityPage";
import SideCard from "@/components/Sidecard";

const services = ["Dashboard", "Listings", "Availability","Bookings"];
const urls = ["/dashboard/realtor", "/dashboard/realtor/house-listings", "/dashboard/realtor/availability", "/dashboard/realtor/bookings"];


const RealtorAvailability = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <Availability />
      </div>
    </div>
  );
};

export default RealtorAvailability;
````

## File: Frontend/src/app/dashboard/realtor/bookings/page.tsx
````typescript
"use client";
import BookingTable from "@/components/availability/BookingTable";
import SideCard from "@/components/Sidecard";

const services = ["Dashboard", "Listings", "Availability","Bookings"];
const urls = ["/dashboard/realtor", "/dashboard/realtor/house-listings", "/dashboard/realtor/availability", "/dashboard/realtor/bookings"];


const RealtorBooking = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <BookingTable />
      </div>
    </div>
  );
};

export default RealtorBooking;
````

## File: Frontend/src/app/dashboard/realtor/edit-listing/[id]/page.tsx
````typescript
"use client";

import { Button } from "@/components/ui/button";
import { useEffect, useState } from "react";
import { useRouter, useParams } from "next/navigation";
import { Card } from "@/components/ui/card";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";

// Helper function to convert a base64 data URL to a File object.
const dataURLtoFile = (dataurl: string, filename: string) => {
  const arr = dataurl.split(",");
  const mimeMatch = arr[0].match(/:(.*?);/);
  if (!mimeMatch) return null;
  const mime = mimeMatch[1];
  const bstr = atob(arr[1]);
  let n = bstr.length;
  const u8arr = new Uint8Array(n);
  while (n--) {
    u8arr[n] = bstr.charCodeAt(n);
  }
  return new File([u8arr], filename, { type: mime });
};

const EditHouseListing = () => {
  const { id } = useParams();
  const router = useRouter();

  const [formData, setFormData] = useState({
    title: "",
    description: "",
    price: "",
    location: "",
    bedrooms: "",
    bathrooms: "",
    squareFeet: "",
    openhouse: false,
    startDate: "",
    endDate: "",
    startTime: "",
    endTime: "",
  });

  // existingImages holds base64 strings from the server and previews for new images.
  const [existingImages, setExistingImages] = useState<string[]>([]);
  // newImages holds File objects from new uploads.
  const [newImages, setNewImages] = useState<File[]>([]);
  const [errorMessage, setErrorMessage] = useState("");
  const [successMessage, setSuccessMessage] = useState("");

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Fetch listing data
  useEffect(() => {
    const fetchData = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok) {
          throw new Error("Failed to get authentication token");
        }
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const response = await fetch(
          `${endpoint}api/protected/house-listing/houselisting/${id}`,
          { headers: { Authorization: `Bearer ${token}` } }
        );
        if (!response.ok) {
          throw new Error("Failed to fetch listing data");
        }
        const data = await response.json();
        setFormData({
          title: data.title || "",
          description: data.description || "",
          price: data.price?.toString() || "",
          location: data.location || "",
          bedrooms: data.bedrooms?.toString() || "",
          bathrooms: data.bathrooms?.toString() || "",
          squareFeet: data.squareFeet?.toString() || "",
          openhouse: data.openhouse || false,
          startDate: data.startdate ? data.startdate.split("T")[0] : "",
          endDate: data.endDate ? data.endDate.split("T")[0] : "",
          startTime: data.startTime || "",
          endTime: data.endTime || "",
        });
        // Assume the API returns houseImages as an array of { base64: string } objects.
        setExistingImages(data.houseImages.map((img: any) => img.base64));
      } catch (error: any) {
        setErrorMessage("Failed to fetch listing data: " + error.message);
      }
    };

    fetchData();
  }, [id, endpoint]);

  // Update form values
  const handleChange = (
    e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>
  ) => {
    const { name, value } = e.target;
    setFormData((prev) => ({ ...prev, [name]: value }));
  };

  // Toggle open house checkbox
  const handleToggleOpenHouse = () => {
    setFormData((prev) => ({ ...prev, openhouse: !prev.openhouse }));
  };

  // Handle new file selection
  const handleFileChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    if (e.target.files) {
      const filesArray = Array.from(e.target.files);
      const newPreviews = filesArray.map((file) => URL.createObjectURL(file));
      setNewImages((prev) => [...prev, ...filesArray]);
      setExistingImages((prev) => [...prev, ...newPreviews]);
    }
  };

  // Remove an image from the preview and newImages if applicable.
  const removeExistingImage = (index: number) => {
    setExistingImages((prev) => prev.filter((_, i) => i !== index));
    if (index >= existingImages.length - newImages.length) {
      const newIndex = index - (existingImages.length - newImages.length);
      setNewImages((prev) => prev.filter((_, i) => i !== newIndex));
    }
  };

  const validateForm = () => {
    if (!formData.title || !formData.price || !formData.location) {
      setErrorMessage("Title, price, and location are required.");
      return false;
    }
    if (isNaN(Number(formData.price)) || Number(formData.price) <= 0) {
      setErrorMessage("Please enter a valid price.");
      return false;
    }
    if (formData.openhouse) {
      if (
        !formData.startDate ||
        !formData.endDate ||
        !formData.startTime ||
        !formData.endTime
      ) {
        setErrorMessage(
          "Start and end date, and time are required for open house."
        );
        return false;
      }
      if (new Date(formData.startDate) > new Date(formData.endDate)) {
        setErrorMessage("Start date must be earlier than end date.");
        return false;
      }
    }
    if (newImages.length > 3) {
      setErrorMessage("You can upload a maximum of 3 new images.");
      return false;
    }
    setErrorMessage("");
    return true;
  };

  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();
    if (!validateForm()) return;

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });
      if (!tokenResponse.ok)
        throw new Error("Failed to get authentication token");
      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      // Convert numeric fields to numbers.
      const numericFields = {
        price: Number(formData.price),
        bedrooms: Number(formData.bedrooms),
        bathrooms: Number(formData.bathrooms),
        // Backend expects key "sqft" for square footage.
        sqft: Number(formData.squareFeet),
      };

      const formDataObj = new FormData();
      formDataObj.append("title", formData.title);
      formDataObj.append("description", formData.description);
      formDataObj.append("location", formData.location);
      formDataObj.append("openhouse", JSON.stringify(formData.openhouse));
      if (formData.openhouse) {
        formDataObj.append("startDate", formData.startDate);
        formDataObj.append("endDate", formData.endDate);
        formDataObj.append("startTime", formData.startTime);
        formDataObj.append("endTime", formData.endTime);
      }
      // Append numeric fields with correct keys.
      formDataObj.append("price", numericFields.price.toString());
      formDataObj.append("bedrooms", numericFields.bedrooms.toString());
      formDataObj.append("bathrooms", numericFields.bathrooms.toString());
      formDataObj.append("sqft", numericFields.sqft.toString());

      // Append existing images from the server.
      const serverImagesCount = existingImages.length - newImages.length;
      const serverImages = existingImages.slice(0, serverImagesCount);
      serverImages.forEach((dataURL, index) => {
        const file = dataURLtoFile(dataURL, `server-image-${index}.png`);
        if (file) formDataObj.append("images", file);
      });

      // Append newly selected images.
      newImages.forEach((image) => {
        formDataObj.append("images", image);
      });

      const response = await fetch(
        `${endpoint}api/protected/house-listing/update-house-listing/${id}`,
        {
          method: "PUT",
          headers: { Authorization: `Bearer ${token}` },
          body: formDataObj,
        }
      );
      if (!response.ok) {
        throw new Error(`Failed to update listing: ${response.statusText}`);
      }
      setSuccessMessage("House listing updated successfully!");
      router.push(`/dashboard/realtor/house-listings/${id}`);
    } catch (error: any) {
      console.error("Error updating listing:", error);
      setErrorMessage("Error updating listing: " + error.message);
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      {/* Back Button */}
      <Link href="/dashboard/realtor/house-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>
      <Card className="shadow-lg">
        <div className="p-6">
          <h1 className="text-2xl font-bold mb-6">Edit House Listing</h1>
          <form onSubmit={handleSubmit}>
            <div className="grid grid-cols-2 gap-4">
              <input
                type="text"
                name="title"
                value={formData.title}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Title"
                required
              />
              <input
                type="text"
                name="price"
                value={formData.price}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Price"
                required
              />
              <input
                type="text"
                name="location"
                value={formData.location}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Location"
                required
              />
              <input
                type="number"
                name="bedrooms"
                value={formData.bedrooms}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Bedrooms"
              />
              <input
                type="number"
                name="bathrooms"
                value={formData.bathrooms}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Bathrooms"
              />
              <input
                type="number"
                name="squareFeet"
                value={formData.squareFeet}
                onChange={handleChange}
                className="border p-2 rounded"
                placeholder="Square Feet"
              />
            </div>

            <textarea
              name="description"
              value={formData.description}
              onChange={handleChange}
              className="border p-2 rounded w-full mt-4"
              placeholder="Description"
            ></textarea>

            <div className="mt-4">
              <label className="flex items-center space-x-2">
                <input
                  type="checkbox"
                  checked={formData.openhouse}
                  onChange={handleToggleOpenHouse}
                />
                <span>Open House</span>
              </label>
            </div>

            {formData.openhouse && (
              <div className="grid grid-cols-2 gap-4 mt-4">
                <input
                  type="date"
                  name="startDate"
                  value={formData.startDate}
                  onChange={handleChange}
                  className="border p-2 rounded"
                  placeholder="Start Date"
                />
                <input
                  type="date"
                  name="endDate"
                  value={formData.endDate}
                  onChange={handleChange}
                  className="border p-2 rounded"
                  placeholder="End Date"
                />
                <input
                  type="time"
                  name="startTime"
                  value={formData.startTime}
                  onChange={handleChange}
                  className="border p-2 rounded"
                  placeholder="Start Time"
                />
                <input
                  type="time"
                  name="endTime"
                  value={formData.endTime}
                  onChange={handleChange}
                  className="border p-2 rounded"
                  placeholder="End Time"
                />
              </div>
            )}

            <div className="mt-4">
              <label className="block font-semibold mb-2">Upload Images</label>
              <input
                type="file"
                multiple
                accept="image/*"
                onChange={handleFileChange}
                className="border p-2 rounded w-full"
              />
              <div className="flex flex-wrap gap-4 mt-4">
                {existingImages.map((image, index) => (
                  <div key={index} className="relative">
                    <img
                      src={image}
                      alt={`House Image ${index}`}
                      className="w-24 h-24 object-cover rounded"
                    />
                    <button
                      type="button"
                      className="absolute top-0 right-0 bg-red-500 text-white p-1 rounded"
                      onClick={() => removeExistingImage(index)}
                    >
                      &times;
                    </button>
                  </div>
                ))}
              </div>
            </div>

            {errorMessage && (
              <p className="text-red-500 mt-4">{errorMessage}</p>
            )}
            {successMessage && (
              <p className="text-blue-500 mt-4">{successMessage}</p>
            )}

            <Button
              type="submit"
              className="bg-blue-600 text-white px-4 py-2 rounded hover:bg-blue-500 mt-4"
            >
              Update Listing
            </Button>
          </form>
        </div>
      </Card>
    </div>
  );
};

export default EditHouseListing;
````

## File: Frontend/src/app/dashboard/realtor/house-listings/[id]/page.tsx
````typescript
"use client";

import { useParams, useRouter } from "next/navigation";
import { useEffect, useState } from "react";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

// Swiper (Carousel)
import { Swiper, SwiperSlide } from "swiper/react";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";

// Icons
import {
  FiArrowLeft,
  FiEdit,
  FiTrash2,
  FiPhoneCall,
  FiMail,
  FiMapPin,
  FiCalendar,
  FiClock,
  FiHome,
  FiGlobe,
  FiDollarSign,
} from "react-icons/fi";
import { FaBed, FaBath } from "react-icons/fa";

const ViewListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [listing, setListing] = useState<any>(null);
  const [userRole, setUserRole] = useState<string | null>(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);

  // Helper: Format dates.
  const formatDate = (dateStr: string) => {
    if (!dateStr) return "N/A";
    return new Date(dateStr).toLocaleDateString();
  };

  useEffect(() => {
    if (id) {
      const fetchListing = async () => {
        try {
          const endpoint = process.env.NEXT_PUBLIC_API_URL;
          const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
          const tokenData = await tokenResponse.json();
          const token = tokenData?.token;
          const role = tokenData?.role;
          if (!token) {
            throw new Error("Invalid authentication token");
          }
          setUserRole(role);
          const response = await fetch(
            `${endpoint}api/protected/house-listing/houselisting/${id}`,
            {
              headers: { Authorization: `Bearer ${token}` },
            }
          );
          if (!response.ok) {
            throw new Error("Failed to fetch listing");
          }
          const data = await response.json();
          setListing(data);
        } catch (err: any) {
          setError(err.message);
        } finally {
          setLoading(false);
        }
      };

      fetchListing();
    }
  }, [id]);

  const handleDelete = async () => {
    if (confirm("Are you sure you want to delete this listing?")) {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) {
          throw new Error("Invalid authentication token");
        }
        const response = await fetch(
          `${endpoint}api/protected/house-listing/delete-house-listing/${id}`,
          {
            method: "DELETE",
            headers: { Authorization: `Bearer ${token}` },
          }
        );
        if (!response.ok) {
          throw new Error("Failed to delete listing");
        }
        alert("Listing deleted successfully");
        router.push("/dashboard/realtor/house-listings");
      } catch (err: any) {
        alert(`Error deleting listing: ${err.message}`);
      }
    }
  };

  if (loading) {
    return <p className="text-center text-lg text-gray-500">Loading...</p>;
  }

  if (error) {
    return <p className="text-center text-red-500 text-lg">Error: {error}</p>;
  }

  if (!listing) {
    return (
      <p className="text-center text-gray-500 text-lg">No listing found</p>
    );
  }

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      {/* Back Button */}
      <Link href="/dashboard/realtor/house-listings">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>

      <div className="flex flex-col md:flex-row gap-6">
        {/* Left: Main Listing Card */}
        <div className="md:w-2/3">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              {/* Image Carousel */}
              {listing.houseImages && listing.houseImages.length > 0 && (
                <Swiper
                  navigation={true}
                  modules={[Navigation]}
                  className="w-full h-96 rounded-lg shadow-lg mb-6"
                >
                  {listing.houseImages.map((image: any, index: number) => (
                    <SwiperSlide key={index}>
                      <img
                        src={image.base64}
                        alt={`House Image ${index + 1}`}
                        className="w-full h-96 object-cover rounded-lg"
                      />
                    </SwiperSlide>
                  ))}
                </Swiper>
              )}

              {/* Title, Price, and Created At */}
              <div className="mb-4">
                <h1 className="text-3xl font-semibold flex items-center gap-2">
                  {listing.title ?? "Untitled"}
                </h1>
                <p className="text-2xl mt-2 text-blue-600 font-bold flex items-center gap-2">
                  <FiDollarSign size={24} />
                  {listing.price ?? "N/A"}
                </p>
                {listing.createdAt && (
                  <p className="mt-2 text-sm text-gray-500">
                    Created At:{" "}
                    {new Date(listing.createdAt).toLocaleDateString()}
                  </p>
                )}
              </div>

              {/* Description */}
              {listing.description && (
                <p className="mb-4">{listing.description}</p>
              )}

              {/* House Attributes */}
              <div className="grid grid-cols-2 md:grid-cols-4 gap-4 mb-4">
                {listing.bedrooms !== null && (
                  <div className="flex items-center gap-2">
                    <FaBed size={20} />
                    <p className="text-lg font-semibold">
                      {listing.bedrooms} Beds
                    </p>
                  </div>
                )}
                {listing.bathrooms !== null && (
                  <div className="flex items-center gap-2">
                    <FaBath size={20} />
                    <p className="text-lg font-semibold">
                      {listing.bathrooms} Baths
                    </p>
                  </div>
                )}
                {listing.squareFeet && (
                  <div className="flex items-center gap-2">
                    <FiHome size={20} />
                    <p className="text-lg font-semibold">
                      {listing.squareFeet} sq ft
                    </p>
                  </div>
                )}
                {listing.location && (
                  <div className="flex items-center gap-2">
                    <FiMapPin size={40} />
                    <p className="text-sm font-semibold">{listing.location}</p>
                  </div>
                )}
              </div>

              {/* Action Buttons */}
              <div className="mt-6 flex flex-wrap gap-4">
                <Link href={`/dashboard/realtor/edit-listing/${id}`}>
                  <Button variant="default" className="flex items-center gap-2">
                    <FiEdit size={18} />
                    Edit Listing
                  </Button>
                </Link>
                <Button
                  variant="destructive"
                  className="flex items-center gap-2"
                  onClick={handleDelete}
                >
                  <FiTrash2 size={18} />
                  Delete Listing
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>

        {/* Right: Landlord / Realtor Info Card */}
        {listing.landlord && (
          <div className="md:w-1/3">
            <Card className="shadow-lg">
              <CardContent className="p-6">
                <h2 className="text-xl font-bold mb-4">Contact</h2>
                {listing.landlord.fullName && (
                  <p className="font-semibold mb-4">
                    {listing.landlord.fullName}
                  </p>
                )}
                {listing.landlord.phoneNo && (
                  <div className="flex items-center gap-2 mb-3">
                    <FiPhoneCall size={18} className="text-blue-500" />
                    <p>{listing.landlord.phoneNo}</p>
                  </div>
                )}
                {listing.landlord.email && (
                  <div className="flex items-center gap-2 mb-3">
                    <FiMail size={18} className="text-blue-500" />
                    <p>{listing.landlord.email}</p>
                  </div>
                )}
                {listing.landlord.realtor && (
                  <>
                    <div className="flex items-center mb-3">
                      <FiMapPin size={18} className="text-red-500 mr-2" />
                      <p>
                        {listing.landlord.realtor.businessName},{" "}
                        {listing.landlord.realtor.businessAddress}
                      </p>
                    </div>
                    <div className="flex items-center mb-3">
                      <FiGlobe size={25} className="mr-2" />
                      <p>{listing.landlord.realtor.portfolioWebsite}</p>
                    </div>
                  </>
                )}
              </CardContent>
            </Card>

            {listing.openhouse && (
              <Card className="shadow-lg mt-2">
                <CardContent className="p-6">
                  <h3 className="text-xl font-semibold mb-2">Open House</h3>
                  <div className="flex items-center gap-2 mb-1">
                    <FiCalendar size={18} />
                    <p className="text-">
                      Start Date: {formatDate(listing.startdate)}
                    </p>
                  </div>
                  <div className="flex items-center gap-2 mb-1">
                    <FiCalendar size={18} />
                    <p>End Date: {formatDate(listing.endDate)}</p>
                  </div>
                  <div className="flex items-center gap-2 mb-1">
                    <FiClock size={18} />
                    <p>Start Time: {listing.startTime ?? "N/A"}</p>
                  </div>
                  <div className="flex items-center gap-2">
                    <FiClock size={18} />
                    <p>End Time: {listing.endTime ?? "N/A"}</p>
                  </div>
                </CardContent>
              </Card>
            )}
          </div>
        )}
      </div>
    </div>
  );
};

export default ViewListing;
````

## File: Frontend/src/app/dashboard/realtor/house-listings/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Listings",
  "Availability",
  "Bookings",
  "Profile",
];
const urls = [
  "/dashboard/realtor",
  "/dashboard/realtor/house-listings",
  "/dashboard/realtor/availability",
  "/dashboard/realtor/bookings",
  "/dashboard/profile",
];

const HousesListing = () => {
  const [houseListings, setHouseListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const houseResponse = await fetch(
          `${endpoint}api/protected/house-listing/all-house-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!houseResponse.ok)
          throw new Error("Failed to fetch house listings");

        const houseData = await houseResponse.json();
        setHouseListings(houseData);
        setFilteredListings(houseData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = houseListings.filter((house) => {
      const openHouseValue = house.openhouse ? "Yes" : "No"; // Convert boolean to string

      return (
        (!filters.location ||
          house.location
            ?.toLowerCase()
            .includes(filters.location.toLowerCase())) &&
        (!filters.price || house.price <= parseFloat(filters.price)) &&
        (!filters.openHouse || openHouseValue === filters.openHouse)
      );
    });

    setFilteredListings(filtered.slice());
  };

  // Debugging UI Update
  useEffect(() => {}, [filteredListings]);

  const houseFiltersConfig = [
    { name: "location", type: "text", placeholder: "Location (e.g. Toronto)" },
    { name: "price", type: "number", placeholder: "Max Price" },
    {
      name: "openHouse",
      type: "select",
      placeholder: "Open-House",
      options: ["Yes", "No"],
    },
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Houses Listing</h2>
          <ReusableFilter
            filtersConfig={houseFiltersConfig}
            onFilterChange={handleFilterChange}
          />
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && filteredListings.length > 0 ? (
          <Listings listings={filteredListings} />
        ) : (
          <p>No houses found.</p>
        )}
      </div>
    </div>
  );
};

export default HousesListing;
````

## File: Frontend/src/app/dashboard/realtor/page.tsx
````typescript
'use client';

import QuickLinks from "@/components/QuickLinks";
import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import { useEffect, useState } from 'react';

export default function DashboardLayout() {
  const [listings, setListings] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  const services = ["Dashboard", "Listings", "Availability","Bookings"];
const urls = ["/dashboard/realtor", "/dashboard/realtor/house-listings", "/dashboard/realtor/availability", "/dashboard/realtor/bookings"];

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        // Fetch token
        const tokenResponse = await fetch(`${endpoint}auth/token`, { credentials: 'include' });

        if (!tokenResponse.ok) {
          throw new Error('Failed to get authentication token');
        }

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;

        if (!token) {
          throw new Error('Invalid authentication token');
        }

        // Fetch house listings
        const response = await fetch(`${endpoint}api/protected/house-listing/by-id-house-listing`, {
          headers: { Authorization: `Bearer ${token}` },
        });

        if (!response.ok) {
          throw new Error('Failed to fetch house listings');
        }

        const data = await response.json();
        setListings(data);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  return (
    <div className="grid grid-cols-12 h-screen"> {/* h-screen for full viewport height */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3"> {/* Fixed SideCard */}
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Realtor Dashboard</h2>
          <QuickLinks links={[
            { label: "Add Listing", href: "realtor/add-listing" },
            { label: "View Listings", href: "realtor/house-listings" },
            { label: "Requests", href: "realtor/availability" },
          ]} />
          <h2 className="text-2xl font-bold mb-6 mt-5">View added listings</h2>
          {loading && <p>Loading...</p>}
          {error && <p>Error: {error}</p>}
          {!loading && !error && listings && <Listings listings={listings} />}
        </div>
      </div>
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/user/bookings/page.tsx
````typescript
"use client";

import SideCard from "@/components/Sidecard";
import BookingView from "@/components/availability/UserBooking";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings"
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings"
];
const UserBooking = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        
        
          <BookingView />
      </div>
    </div>
  );
};

export default UserBooking;
````

## File: Frontend/src/app/dashboard/user/cars/car-listings/[id]/page.tsx
````typescript
"use client";

import { useParams, useRouter } from "next/navigation";
import { useEffect, useState } from "react";
import Link from "next/link";

import { Button } from "@/components/ui/button";
import {
  FiArrowLeft,
  FiCalendar,
  FiDroplet,
  FiSettings,
  FiUsers,
  FiPhoneCall,
  FiMail,
  FiMapPin,
  FiDollarSign,
  FiHeart,
} from "react-icons/fi";
import { MdSpeed, MdFormatPaint } from "react-icons/md";
import { Swiper, SwiperSlide } from "swiper/react";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";
import { Card, CardContent } from "@/components/ui/card";

const ViewCarListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [listing, setListing] = useState<any>(null);
  const [userRole, setUserRole] = useState<string | null>(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const checkIfAnyDateIsFuture = (data) => {
    // Get current UTC time
    const currentTime = new Date();

    // Use Array.some() to stop as soon as a future date is found
    const isFuture = data.some((item) => {
      // Validate if endDate exists and is a valid date
      if (!item.endDate) return false;

      // Convert endDate to a Date object
      const endDateUTC = new Date(item.endDate);

      // Check if endDate is valid and greater than currentTime
      return !isNaN(endDateUTC.getTime()) && endDateUTC > currentTime;
    });

    return isFuture;
  };

  useEffect(() => {
    if (id) {
      const fetchListing = async () => {
        try {
          // Fetch token
          const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
          const tokenData = await tokenResponse.json();
          const token = tokenData?.token;
          const role = tokenData?.role;
          if (!token) {
            throw new Error("Invalid authentication token");
          }
          setUserRole(role);

          // Fetch car listing
          const response = await fetch(
            `${endpoint}api/protected/car-listing/carlisting/${id}`,
            {
              headers: { Authorization: `Bearer ${token}` },
            }
          );
          if (!response.ok) {
            throw new Error("Failed to fetch car listing");
          }
          const data = await response.json();
          setListing(data);
        } catch (err: any) {
          setError(err.message);
        } finally {
          setLoading(false);
        }
      };
      fetchListing();
    }
  });

  // Helper functions to format dealership info
  const formatFinancingOptions = (optionsStr: string) => {
    return optionsStr
      .replace(/[{}"]/g, "")
      .split(",")
      .map((o) => o.trim());
  };

  const formatShowroomLocations = (locationsStr: string) => {
    return locationsStr.replace(/[{}"]/g, "");
  };

  if (loading) {
    return <p className="text-center text-lg text-gray-500">Loading...</p>;
  }
  if (error) {
    return <p className="text-center text-red-500 text-lg">Error: {error}</p>;
  }
  if (!listing) {
    return (
      <p className="text-center text-gray-500 text-lg">No car listing found</p>
    );
  }

  const handleContactSeller = async (listingId: number, type: string) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData?.token;

      const response = await fetch(
        `${endpoint}api/protected/appointment/booking-status?listingId=${listingId}&type=${type}`,
        {
          method: "GET",
          headers: {
            "Content-Type": "application/json",
            Authorization: `Bearer ${token}`,
          },
        }
      );

      if (response.status === 200) {
        const data = await response.json();
        if (checkIfAnyDateIsFuture(data.booking)) {
          alert("You have already booked an appointment with this seller");
        } else {
          alert("Action Pending from Consultant");
        }
      } else {
        router.push(`/dashboard/user/slots/${listingId}/${type}`);
      }
    } catch (error) {
      console.error("Error contacting seller:", error);
      alert("An error occurred while processing your request.");
    }
  };

  const handleSaveListing = async (listingId: number) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData?.token;
      const response = await fetch(
        `${endpoint}api/protected/car-listing/add-to-favourites`,
        {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            Authorization: `Bearer ${token}`,
          },
          body: JSON.stringify({
            listingId: listingId,
          }),
        }
      );

      if (response.status === 200) {
        const data = await response.json();
      }
    } catch (error) {
      console.error("Error saving listing:", error);
      alert("An error occurred while processing your request.");
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      <Link href="/dashboard/user">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>

      <div className="flex flex-col md:flex-row gap-6">
        {/* Main Listing Card */}
        <div className="md:w-2/3">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              {/* Image Carousel */}
              {listing.carImages && listing.carImages.length > 0 && (
                <Swiper
                  navigation={true}
                  modules={[Navigation]}
                  className="w-full h-96 rounded-lg shadow-lg mb-6"
                >
                  {listing.carImages.map((image, index) => (
                    <SwiperSlide key={index}>
                      <img
                        src={image.base64}
                        alt={`Car Image ${index + 1}`}
                        className="w-full h-96 object-cover rounded-lg"
                      />
                    </SwiperSlide>
                  ))}
                </Swiper>
              )}
              {/* Car Details */}
              <div className="mb-4">
                <h1 className="text-3xl font-semibold">
                  {listing.model} - {listing.make}
                </h1>
                {listing.createdAt && (
                  <p className="mt-2 text-sm text-gray-500">
                    Created At:{" "}
                    {new Date(listing.createdAt).toLocaleDateString()}
                  </p>
                )}
                <p className="text-2xl mt-2 text-blue-600 font-bold flex items-center gap-1">
                  <FiDollarSign size={24} />
                  {listing.price ?? "N/A"}
                </p>
              </div>
              {/* Specifications */}
              <div className="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-3 gap-4">
                <div className="flex items-center gap-1">
                  <FiCalendar size={20} />
                  <p className="text-lg font-semibold">
                    {listing.year ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <MdSpeed size={20} />
                  <p className="text-lg font-semibold">
                    {listing.mileage ? `${listing.mileage} km` : "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiSettings size={20} />
                  <p className="text-lg font-semibold">
                    {listing.transmission ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiDroplet size={20} />
                  <p className="text-lg font-semibold">
                    {listing.fuelType ?? "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <FiUsers size={20} />
                  <p className="text-lg font-semibold">
                    {listing.noOfSeats ? `${listing.noOfSeats} Seats` : "N/A"}
                  </p>
                </div>
                <div className="flex items-center gap-1">
                  <MdFormatPaint size={20} />
                  <p className="text-lg font-semibold">
                    {listing.exteriorColor ?? "N/A"}
                  </p>
                </div>
              </div>

              {/* Action Buttons */}
              <div className="mt-6 flex flex-wrap gap-4">
                {/* Public buttons */}
                <Button
                  variant="outline"
                  className="flex items-center gap-2"
                  onClick={() => handleContactSeller(listing.id, "car")}
                >
                  <FiPhoneCall size={18} />
                  Contact Seller
                </Button>

                <Button
                  variant="secondary"
                  className="flex items-center gap-2"
                  onClick={() => handleSaveListing(listing.id)}
                >
                  <FiHeart size={18} />
                  Save Listing
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>

        {/* Separate Dealership Info Container */}
        {listing.dealership && (
          <div className="md:w-1/3">
            <Card className="shadow-lg">
              <CardContent className="p-6">
                <h2 className="text-xl font-bold mb-4">Contact Details: </h2>
                <div className="mb-3">
                  <p className="font-semibold">{listing.dealership.fullName}</p>
                </div>
                <div className="flex items-center mb-3">
                  <FiPhoneCall size={18} className="text-blue-500 mr-2" />
                  <p>{listing.dealership.phoneNo}</p>
                </div>
                <div className="flex items-center mb-3">
                  <FiMail size={18} className="text-blue-500 mr-2" />
                  <p>{listing.dealership.email}</p>
                </div>
                {listing.dealership.carDealership && (
                  <>
                    <div className="flex items-center mb-3">
                      <FiMapPin size={18} className="text-red-500 mr-2" />
                      <div>
                        <p className="text-lg">
                          {listing.dealership.carDealership.businessName}
                        </p>
                        <p className="text-lg">
                          {formatShowroomLocations(
                            listing.dealership.carDealership.showroomLocations
                          )}
                        </p>
                      </div>
                    </div>
                    <div className="mb-3">
                      <ul className="list-disc list-inside">
                        {formatFinancingOptions(
                          listing.dealership.carDealership.financingOptions
                        ).map((option, idx) => (
                          <li key={idx} className="text-lg">
                            {option}
                          </li>
                        ))}
                      </ul>
                    </div>
                  </>
                )}
              </CardContent>
            </Card>
          </div>
        )}
      </div>
    </div>
  );
};

export default ViewCarListing;
````

## File: Frontend/src/app/dashboard/user/cars/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];
const CarsListing = () => {
  const [carListings, setCarListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);
  const [refresh, setRefresh] = useState(false);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const carResponse = await fetch(
          `${endpoint}api/protected/car-listing/all-car-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!carResponse.ok) throw new Error("Failed to fetch car listings");

        const carData = await carResponse.json();
        setCarListings(carData);
        setFilteredListings(carData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);
  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = carListings.filter((car) => {
      return (
        (!filters.make ||
          car.make?.toLowerCase().includes(filters.make.toLowerCase())) &&
        (!filters.model ||
          car.model?.toLowerCase().includes(filters.model.toLowerCase())) &&
        (!filters.price || car.price <= parseFloat(filters.price))
      );
    });

    setFilteredListings(filtered.slice());
  };

  // Debugging UI Update
  useEffect(() => {}, [filteredListings]);

  const carFiltersConfig = [
    { name: "make", type: "text", placeholder: "Make (e.g. Toyota)" },
    { name: "model", type: "text", placeholder: "Model (e.g. Corolla)" },
    { name: "price", type: "number", placeholder: "Max Price" },
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Cars Listing</h2>
          <ReusableFilter
            filtersConfig={carFiltersConfig}
            onFilterChange={handleFilterChange}
          />
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && filteredListings.length > 0 ? (
          <Listings key={refresh} listings={filteredListings} />
        ) : (
          <p>No cars found.</p>
        )}
      </div>
    </div>
  );
};

export default CarsListing;
````

## File: Frontend/src/app/dashboard/user/consultant/page.tsx
````typescript
"use client";

import ConsultantCarousel from "@/components/consultant/ConsultantCarousel";
import SideCard from "@/components/Sidecard";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];
const ConsultantPage = () => {
  const [consultanatListings, setConsultanatListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const consultantResponse = await fetch(
          `${endpoint}api/protected/consultants/view-consultant`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!consultantResponse.ok)
          throw new Error("Failed to fetch car listings");

        const consultantData = await consultantResponse.json();
        setConsultanatListings(consultantData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Consultants</h2>
          {/* <ReusableFilter filtersConfig={carFiltersConfig} onFilterChange={handleFilterChange} /> */}
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && consultanatListings && (
          <ConsultantCarousel
            consultants={consultanatListings.consultants || []}
          />
        )}
      </div>
    </div>
  );
};

export default ConsultantPage;
````

## File: Frontend/src/app/dashboard/user/favourites-car/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];

const FavouriteCars = () => {
  const [carListings, setCarListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchFavourites = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenRes = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenRes.ok) throw new Error("Failed to get token");

        const { token } = await tokenRes.json();
        if (!token) throw new Error("Token missing");

        const carRes = await fetch(
          `${endpoint}api/protected/car-listing/favourites`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!carRes.ok) throw new Error("Failed to fetch favourite cars");

        const data = await carRes.json();
        setCarListings(data);
        setFilteredListings(data);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchFavourites();
  }, []);

  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = carListings.filter((car) => {
      return (
        (!filters.make ||
          car.make?.toLowerCase().includes(filters.make.toLowerCase())) &&
        (!filters.model ||
          car.model?.toLowerCase().includes(filters.model.toLowerCase())) &&
        (!filters.price || car.price <= parseFloat(filters.price))
      );
    });

    setFilteredListings(filtered.slice());
  };

  const carFiltersConfig = [
    { name: "make", type: "text" as const, placeholder: "Make (e.g. Toyota)" },
    {
      name: "model",
      type: "text" as const,
      placeholder: "Model (e.g. Corolla)",
    },
    { name: "price", type: "number" as const, placeholder: "Max Price" },
  ];

  return (
    <div>
      <div className="container mx-auto">
        <h2 className="text-2xl font-bold mb-6 mt-4">Favourite Cars</h2>
        <ReusableFilter
          filtersConfig={carFiltersConfig}
          onFilterChange={handleFilterChange}
        />
      </div>
      {loading && <p>Loading...</p>}
      {error && <p className="text-red-500">Error: {error}</p>}
      {!loading && !error && filteredListings.length > 0 ? (
        <Listings listings={filteredListings} />
      ) : (
        <p>No favourite cars found.</p>
      )}
    </div>
  );
};

export default FavouriteCars;
````

## File: Frontend/src/app/dashboard/user/favourites-house/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];

const FavouriteHouse = () => {
  const [houseListings, setHouseListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchFavourites = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenRes = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenRes.ok) throw new Error("Failed to get authentication token");

        const { token } = await tokenRes.json();
        if (!token) throw new Error("Invalid token");

        const response = await fetch(
          `${endpoint}api/protected/house-listing/favourites`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!response.ok) throw new Error("Failed to fetch favourite houses");

        const data = await response.json();
        setHouseListings(data);
        setFilteredListings(data);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchFavourites();
  }, []);

  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = houseListings.filter((house) => {
      const openHouseValue = house.openhouse ? "Yes" : "No";

      return (
        (!filters.location ||
          house.location
            ?.toLowerCase()
            .includes(filters.location.toLowerCase())) &&
        (!filters.price || house.price <= parseFloat(filters.price)) &&
        (!filters.openHouse || openHouseValue === filters.openHouse)
      );
    });

    setFilteredListings(filtered);
  };

  const houseFiltersConfig = [
    { name: "location", type: "text", placeholder: "Location (e.g. Toronto)" },
    { name: "price", type: "number", placeholder: "Max Price" },
    {
      name: "openHouse",
      type: "select",
      placeholder: "Open-House",
      options: ["Yes", "No"],
    },
  ];

  return (
    <div>
      <div className="container mx-auto">
        <h2 className="text-2xl font-bold mb-6 mt-4">Favourite Houses</h2>
        <ReusableFilter
          filtersConfig={houseFiltersConfig}
          onFilterChange={handleFilterChange}
        />
      </div>
      {loading && <p>Loading...</p>}
      {error && <p className="text-red-500">Error: {error}</p>}
      {!loading && !error && filteredListings.length > 0 ? (
        <Listings listings={filteredListings} />
      ) : (
        <p>No favourite houses found.</p>
      )}
    </div>
  );
};

export default FavouriteHouse;
````

## File: Frontend/src/app/dashboard/user/homes/house-listings/[id]/page.tsx
````typescript
"use client";

import { useParams, useRouter } from "next/navigation";
import { useEffect, useState } from "react";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

// Swiper (Carousel)
import { Swiper, SwiperSlide } from "swiper/react";
import "swiper/css";
import "swiper/css/navigation";
import { Navigation } from "swiper/modules";

// Icons
import {
  FiArrowLeft,
  FiEdit,
  FiTrash2,
  FiPhoneCall,
  FiMail,
  FiMapPin,
  FiCalendar,
  FiClock,
  FiHome,
  FiGlobe,
  FiDollarSign,
  FiHeart,
} from "react-icons/fi";
import { FaBed, FaBath } from "react-icons/fa";

const ViewListing = () => {
  const { id } = useParams();
  const router = useRouter();
  const [listing, setListing] = useState<any>(null);
  const [userRole, setUserRole] = useState<string | null>(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // Helper: Format dates.
  const formatDate = (dateStr: string) => {
    if (!dateStr) return "N/A";
    return new Date(dateStr).toLocaleDateString();
  };

  const checkIfAnyDateIsFuture = (data) => {
    // Get current UTC time
    const currentTime = new Date();

    // Use Array.some() to stop as soon as a future date is found
    const isFuture = data.some((item) => {
      // Validate if endDate exists and is a valid date
      if (!item.endDate) return false;

      // Convert endDate to a Date object
      const endDateUTC = new Date(item.endDate);

      // Check if endDate is valid and greater than currentTime
      return !isNaN(endDateUTC.getTime()) && endDateUTC > currentTime;
    });

    return isFuture;
  };

  useEffect(() => {
    if (id) {
      const fetchListing = async () => {
        try {
          const endpoint = process.env.NEXT_PUBLIC_API_URL;
          const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
          const tokenData = await tokenResponse.json();
          const token = tokenData?.token;
          const role = tokenData?.role;
          if (!token) {
            throw new Error("Invalid authentication token");
          }
          setUserRole(role);
          const response = await fetch(
            `${endpoint}api/protected/house-listing/houselisting/${id}`,
            {
              headers: { Authorization: `Bearer ${token}` },
            }
          );
          if (!response.ok) {
            throw new Error("Failed to fetch listing");
          }
          const data = await response.json();
          setListing(data);
        } catch (err: any) {
          setError(err.message);
        } finally {
          setLoading(false);
        }
      };

      fetchListing();
    }
  }, [id]);

  const handleDelete = async () => {
    if (confirm("Are you sure you want to delete this listing?")) {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) {
          throw new Error("Invalid authentication token");
        }
        const response = await fetch(
          `${endpoint}api/protected/house-listing/delete-house-listing/${id}`,
          {
            method: "DELETE",
            headers: { Authorization: `Bearer ${token}` },
          }
        );
        if (!response.ok) {
          throw new Error("Failed to delete listing");
        }
        alert("Listing deleted successfully");
        router.push("/dashboard/realtor/house-listings");
      } catch (err: any) {
        alert(`Error deleting listing: ${err.message}`);
      }
    }
  };

  if (loading) {
    return <p className="text-center text-lg text-gray-500">Loading...</p>;
  }

  if (error) {
    return <p className="text-center text-red-500 text-lg">Error: {error}</p>;
  }

  if (!listing) {
    return (
      <p className="text-center text-gray-500 text-lg">No listing found</p>
    );
  }

  const handleContactSeller = async (listingId: number, type: string) => {
    const tokenResponse = await fetch(`${endpoint}auth/token`, {
      credentials: "include",
    });
    if (!tokenResponse.ok) {
      throw new Error("Failed to get authentication token");
    }
    const tokenData = await tokenResponse.json();
    const token = tokenData?.token;
    const response = await fetch(
      `${endpoint}api/protected/appointment/booking-status?listingId=${listingId}&type=${type}`,
      {
        method: "GET",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
      }
    );

    if (response.status === 200) {
      const data = await response.json();
      if (checkIfAnyDateIsFuture(data.booking)) {
        alert("You have already booked an appointment with this seller");
      } else {
        alert("Action Pending from Realtor");
      }
    } else {
      router.push(`/dashboard/user/slots/${listingId}/${type}`);
    }
  };

  const handleSaveListing = async (listingId: number) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData?.token;
      const response = await fetch(
        `${endpoint}api/protected/house-listing/add-to-favourites`,
        {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            Authorization: `Bearer ${token}`,
          },
          body: JSON.stringify({
            listingId: listingId,
          }),
        }
      );

      if (response.status === 200) {
        const data = await response.json();
      }
    } catch (error) {
      console.error("Error saving listing:", error);
      alert("An error occurred while processing your request.");
    }
  };

  return (
    <div className="max-w-5xl mx-auto p-6 mt-10">
      {/* Back Button */}
      <Link href="/dashboard/user/">
        <Button variant="ghost" className="flex items-center gap-2 mb-4">
          <FiArrowLeft size={18} />
          Back to Listings
        </Button>
      </Link>

      <div className="flex flex-col md:flex-row gap-6">
        {/* Left: Main Listing Card */}
        <div className="md:w-2/3">
          <Card className="shadow-lg">
            <CardContent className="p-6">
              {/* Image Carousel */}
              {listing.houseImages && listing.houseImages.length > 0 && (
                <Swiper
                  navigation={true}
                  modules={[Navigation]}
                  className="w-full h-96 rounded-lg shadow-lg mb-6"
                >
                  {listing.houseImages.map((image: any, index: number) => (
                    <SwiperSlide key={index}>
                      <img
                        src={image.base64}
                        alt={`House Image ${index + 1}`}
                        className="w-full h-96 object-cover rounded-lg"
                      />
                    </SwiperSlide>
                  ))}
                </Swiper>
              )}

              {/* Title, Price, and Created At */}
              <div className="mb-4">
                <h1 className="text-3xl font-semibold flex items-center gap-2">
                  {listing.title ?? "Untitled"}
                </h1>
                <p className="text-2xl mt-2 text-blue-600 font-bold flex items-center gap-2">
                  <FiDollarSign size={24} />
                  {listing.price ?? "N/A"}
                </p>
                {listing.createdAt && (
                  <p className="mt-2 text-sm text-gray-500">
                    Created At:{" "}
                    {new Date(listing.createdAt).toLocaleDateString()}
                  </p>
                )}
              </div>

              {/* Description */}
              {listing.description && (
                <p className="mb-4">{listing.description}</p>
              )}

              {/* House Attributes */}
              <div className="grid grid-cols-2 md:grid-cols-4 gap-4 mb-4">
                {listing.bedrooms !== null && (
                  <div className="flex items-center gap-2">
                    <FaBed size={20} />
                    <p className="text-lg font-semibold">
                      {listing.bedrooms} Beds
                    </p>
                  </div>
                )}
                {listing.bathrooms !== null && (
                  <div className="flex items-center gap-2">
                    <FaBath size={20} />
                    <p className="text-lg font-semibold">
                      {listing.bathrooms} Baths
                    </p>
                  </div>
                )}
                {listing.squareFeet && (
                  <div className="flex items-center gap-2">
                    <FiHome size={20} />
                    <p className="text-lg font-semibold">
                      {listing.squareFeet} sq ft
                    </p>
                  </div>
                )}
                {listing.location && (
                  <div className="flex items-center gap-2">
                    <FiMapPin size={40} />
                    <p className="text-sm font-semibold">{listing.location}</p>
                  </div>
                )}
              </div>

              {/* Action Buttons */}
              <div className="mt-6 flex flex-wrap gap-4">
                {/* Public buttons */}
                <Button
                  variant="outline"
                  className="flex items-center gap-2"
                  onClick={() => handleContactSeller(listing.id, "house")}
                >
                  <FiPhoneCall size={18} />
                  Contact Seller
                </Button>

                <Button
                  variant="secondary"
                  className="flex items-center gap-2"
                  onClick={() => handleSaveListing(listing.id)}
                >
                  <FiHeart size={18} />
                  Save Listing
                </Button>
              </div>
            </CardContent>
          </Card>
        </div>

        {/* Right: Landlord / Realtor Info Card */}
        {listing.landlord && (
          <div className="md:w-1/3">
            <Card className="shadow-lg">
              <CardContent className="p-6">
                <h2 className="text-xl font-bold mb-4">Contact</h2>
                {listing.landlord.fullName && (
                  <p className="font-semibold mb-4">
                    {listing.landlord.fullName}
                  </p>
                )}
                {listing.landlord.phoneNo && (
                  <div className="flex items-center gap-2 mb-3">
                    <FiPhoneCall size={18} className="text-blue-500" />
                    <p>{listing.landlord.phoneNo}</p>
                  </div>
                )}
                {listing.landlord.email && (
                  <div className="flex items-center gap-2 mb-3">
                    <FiMail size={18} className="text-blue-500" />
                    <p>{listing.landlord.email}</p>
                  </div>
                )}
                {listing.landlord.realtor && (
                  <>
                    <div className="flex items-center mb-3">
                      <FiMapPin size={18} className="text-red-500 mr-2" />
                      <p>
                        {listing.landlord.realtor.businessName},{" "}
                        {listing.landlord.realtor.businessAddress}
                      </p>
                    </div>
                    <div className="flex items-center mb-3">
                      <FiGlobe size={25} className="mr-2" />
                      <p>{listing.landlord.realtor.portfolioWebsite}</p>
                    </div>
                  </>
                )}
              </CardContent>
            </Card>

            {listing.openhouse && (
              <Card className="shadow-lg mt-2">
                <CardContent className="p-6">
                  <h3 className="text-xl font-semibold mb-2">Open House</h3>
                  <div className="flex items-center gap-2 mb-1">
                    <FiCalendar size={18} />
                    <p className="text-">
                      Start Date: {formatDate(listing.startdate)}
                    </p>
                  </div>
                  <div className="flex items-center gap-2 mb-1">
                    <FiCalendar size={18} />
                    <p>End Date: {formatDate(listing.endDate)}</p>
                  </div>
                  <div className="flex items-center gap-2 mb-1">
                    <FiClock size={18} />
                    <p>Start Time: {listing.startTime ?? "N/A"}</p>
                  </div>
                  <div className="flex items-center gap-2">
                    <FiClock size={18} />
                    <p>End Time: {listing.endTime ?? "N/A"}</p>
                  </div>
                </CardContent>
              </Card>
            )}
          </div>
        )}
      </div>
    </div>
  );
};

export default ViewListing;
````

## File: Frontend/src/app/dashboard/user/homes/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];
const HousesListing = () => {
  const [houseListings, setHouseListings] = useState([]);
  const [filteredListings, setFilteredListings] = useState([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        if (!token) throw new Error("Invalid authentication token");

        const houseResponse = await fetch(
          `${endpoint}api/protected/house-listing/all-house-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!houseResponse.ok)
          throw new Error("Failed to fetch house listings");

        const houseData = await houseResponse.json();
        setHouseListings(houseData);
        setFilteredListings(houseData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  const handleFilterChange = (filters: Record<string, string>) => {
    const filtered = houseListings.filter((house) => {
      const openHouseValue = house.openhouse ? "Yes" : "No"; // Convert boolean to string

      return (
        (!filters.location ||
          house.location
            ?.toLowerCase()
            .includes(filters.location.toLowerCase())) &&
        (!filters.price || house.price <= parseFloat(filters.price)) &&
        (!filters.openHouse || openHouseValue === filters.openHouse)
      );
    });

    setFilteredListings(filtered.slice());
  };
  
  // Debugging UI Update
  useEffect(() => {
  }, [filteredListings]);

  


  const houseFiltersConfig = [
    { name: "location", type: "text", placeholder: "Location (e.g. Toronto)" },
    { name: "price", type: "number", placeholder: "Max Price" },
    {
      name: "openHouse",
      type: "select",
      placeholder: "Open-House",
      options: ["Yes", "No"],
    },
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">Houses Listing</h2>
          <ReusableFilter
            filtersConfig={houseFiltersConfig}
            onFilterChange={handleFilterChange}
          />
        </div>
        {loading && <p>Loading...</p>}
        {error && <p>Error: {error}</p>}
        {!loading && !error && filteredListings.length > 0 ? (
          <Listings listings={filteredListings} />
        ) : (
          <p>No houses found.</p>
        )}
      </div>
    </div>
  );
};

export default HousesListing;
````

## File: Frontend/src/app/dashboard/user/page.tsx
````typescript
"use client";

import QuickLinks from "@/components/QuickLinks";
import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import { useEffect, useState } from "react";

export default function DashboardLayout() {
  const [carListings, setCarListings] = useState(null);
  const [houseListings, setHouseListings] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    const fetchListings = async () => {
      try {
        const endpoint = process.env.NEXT_PUBLIC_API_URL;

        // Fetch token
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });

        if (!tokenResponse.ok) {
          throw new Error("Failed to get authentication token");
        }

        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;

        if (!token) {
          throw new Error("Invalid authentication token");
        }

        // Fetch house listings
        const houseResponse = await fetch(
          `${endpoint}api/protected/house-listing/all-house-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!houseResponse.ok) {
          throw new Error("Failed to fetch house listings");
        }

        const houseData = await houseResponse.json();
        setHouseListings(houseData);

        // Fetch car listings
        const carResponse = await fetch(
          `${endpoint}api/protected/car-listing/all-car-listing`,
          {
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        if (!carResponse.ok) {
          throw new Error("Failed to fetch car listings");
        }

        const carData = await carResponse.json();
        setCarListings(carData);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    };

    fetchListings();
  }, []);

  const services = [
    "Dashboard",
    "Explore Homes",
    "Explore Cars",
    "Book Consultation",
    "Bookings",
  ];
  const urls = [
    "/dashboard/user",
    "/dashboard/user/homes",
    "/dashboard/user/cars",
    "/dashboard/user/consultant",
    "/dashboard/user/bookings",
  ];

  return (
    <div className="grid grid-cols-12 h-full">
      {" "}
      {/* h-screen for full viewport height */}
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        {" "}
        {/* Fixed SideCard */}
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <div className="container mx-auto">
          <h2 className="text-2xl font-bold mb-6 mt-4">User Dashboard</h2>
          <QuickLinks
            links={[
              { label: "Profile Settings", href: "/dashboard/user/profile" },
              { label: "Saved Listings", href: "/dashboard/user/saved" },
              { label: "Booking History", href: "/dashboard/user/bookings" },
            ]}
          />
          <h2 className="text-2xl font-bold mb-6 mt-4">
            Explore recent home listings
          </h2>
          {loading && <p>Loading...</p>}
          {error && <p>Error: {error}</p>}
          {!loading && !error && houseListings && (
            <Listings listings={houseListings} />
          )}
          <h2 className="text-2xl font-bold mb-6 mt-4">
            Explore recent car listings
          </h2>
          {!loading && !error && carListings && (
            <Listings listings={carListings} />
          )}
        </div>
      </div>
    </div>
  );
}
````

## File: Frontend/src/app/dashboard/user/profile/page.tsx
````typescript
// /app/profile/page.tsx
"use client";

import React, { useEffect, useState } from "react";
import SideCard from "@/components/Sidecard";
import UserProfile from "@/components/UserProfile";

interface UserData {
  fullName: string;
  DOB: string;
  phoneNo: string;
  email: string;
  alreadyInCanada?: boolean | null;
  statusInCanada?: string | null;
  countryOfOrigin?: string | null;
  currentLocation?: string | null;
}

const ProfilePage: React.FC = () => {
  const [userData, setUserData] = useState<UserData | null>(null);
  const [loading, setLoading] = useState<boolean>(true);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  useEffect(() => {
    const fetchUserData = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
            credentials: "include",
          });
    
          if (!tokenResponse.ok) {
            throw new Error("Failed to get authentication token");
          }
    
          const tokenData = await tokenResponse.json();
          const token = tokenData.token;
          const response = await fetch(`${endpoint}api/protected/profile`, {
            method: "GET",
            headers: {
              Authorization: `Bearer ${token}`,
            },
          });
       
        if (!response.ok) {
          throw new Error("Failed to fetch user data");
        }
        const data = await response.json();
        setUserData(data);
      } catch (error) {
        console.error("Error fetching user data:", error);
      } finally {
        setLoading(false);
      }
    };

    fetchUserData();
  }, []);

  const services = [
    "Dashboard",
    "Explore Homes",
    "Explore Cars",
    "Book Consultation",
    "Bookings"
  ];
  const urls = [
    "/dashboard/user",
    "/dashboard/user/homes",
    "/dashboard/user/cars",
    "/dashboard/user/consultant",
    "/dashboard/user/bookings"
  ];

  if (loading) {
    return <p className="text-center mt-10">Loading...</p>;
  }

  if (!userData) {
    return <p className="text-center mt-10">No user data available</p>;
  }

  return(
    <div className="grid grid-cols-12 h-full">
          <div className="col-span-12 md:col-span-3 mt-3 p-3">
            <SideCard services={services} title="Services" urls={urls} />
          </div>
          <div className="col-span-12 md:col-span-9 p-5">
            
            
          <UserProfile userData={userData} />;
          </div>
        </div>
  ) 
};

export default ProfilePage;
````

## File: Frontend/src/app/dashboard/user/saved/page.tsx
````typescript
"use client";

import Listings from "@/components/Listings";
import SideCard from "@/components/Sidecard";
import ReusableFilter from "@/components/Filter";
import React, { useEffect, useState } from "react";
import { Tabs, TabsContent, TabsList, TabsTrigger } from "@/components/ui/tabs";
import FavouriteCars from "../favourites-car/page";
import FavouriteHouse from "../favourites-house/page";

const services = [
  "Dashboard",
  "Explore Homes",
  "Explore Cars",
  "Book Consultation",
  "Bookings",
];
const urls = [
  "/dashboard/user",
  "/dashboard/user/homes",
  "/dashboard/user/cars",
  "/dashboard/user/consultant",
  "/dashboard/user/bookings",
];

const Saved = () => {
  return (
    <div className="grid grid-cols-12 h-full">
      <div className="col-span-12 md:col-span-3 mt-3 p-3">
        <SideCard services={services} title="Services" urls={urls} />
      </div>
      <div className="col-span-12 md:col-span-9 p-5">
        <Tabs defaultValue="account" className="">
          <TabsList className="grid w-full grid-cols-2">
            <TabsTrigger value="cars">Cars</TabsTrigger>
            <TabsTrigger value="houses">Houses</TabsTrigger>
          </TabsList>
          <TabsContent value="cars">
            <FavouriteCars />
          </TabsContent>
          <TabsContent value="houses">
            <FavouriteHouse />
          </TabsContent>
          <TabsContent value="consultants">No Saved Consultant</TabsContent>
        </Tabs>
      </div>
    </div>
  );
};

export default Saved;
````

## File: Frontend/src/app/dashboard/user/slots/[listingId]/[type]/page.tsx
````typescript
"use client";

import { useParams } from "next/navigation";
import AppointmentBooking from "@/components/availability/AppointmentBooking";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";
import { Button } from "@/components/ui/button";

const AppointmentBookingPage = () => {
  const params = useParams();
  const listingId = params.listingId as string;
  const type = params.type as "car" | "house";

  if (!listingId || !type) {
    return (
      <div className="flex flex-col items-center justify-center h-screen text-gray-500">
        <p className="text-lg">Invalid request. Missing parameters.</p>
        <Link href="/dashboard/user">
          <Button variant="outline" className="mt-4">
            Back to Dashboard
          </Button>
        </Link>
      </div>
    );
  }
  const backLink =
  type === "car"
    ? `/dashboard/user/cars/car-listings/${listingId}`
    : `/dashboard/user/homes/house-listings/${listingId}`;

  return (
    <div className="max-w-4xl mx-auto p-6 mt-10 bg-white shadow-lg rounded-lg">
      {/* Back Button */}
      
      <Link href={backLink}>
        <Button variant="ghost" className="flex items-center gap-2 mb-4 text-gray-600 hover:text-gray-900">
          <FiArrowLeft size={20} />
          <span className="font-medium">Back to Listings</span>
        </Button>
      </Link>

      {/* Header Section */}
      <div className="text-center mb-6">
        <h1 className="text-3xl font-semibold text-gray-800">📅 Book an Appointment</h1>
        <p className="text-gray-600 mt-2">Select a time slot to schedule your appointment.</p>
      </div>

      {/* Appointment Booking Component */}
      <div className="bg-gray-100 p-5 rounded-lg shadow-sm">
        <AppointmentBooking listingId={listingId} type={type} />
      </div>
    </div>
  );
};

export default AppointmentBookingPage;
````

## File: Frontend/src/app/dashboard/user/slots/consultant/[consultantId]/page.tsx
````typescript
"use client";

import { useParams } from "next/navigation";
import AppointmentBooking from "@/components/availability/AppointmentBooking";
import Link from "next/link";
import { FiArrowLeft } from "react-icons/fi";
import { Button } from "@/components/ui/button";

const AppointmentBookingCPage = () => {
  const params = useParams();
  const consultantId = params.consultantId as string;

  if (!consultantId) {
    return (
      <div className="flex flex-col items-center justify-center h-screen text-gray-500">
        <p className="text-lg">Invalid request. Missing parameters.</p>
        <Link href="/dashboard/user">
          <Button variant="outline" className="mt-4">
            Back to Dashboard
          </Button>
        </Link>
      </div>
    );
  }
  const backLink =
   `/dashboard/user/consultant`

  return (
    <div className="max-w-4xl mx-auto p-6 mt-10 bg-white shadow-lg rounded-lg">
      {/* Back Button */}
      
      <Link href={backLink}>
        <Button variant="ghost" className="flex items-center gap-2 mb-4 text-gray-600 hover:text-gray-900">
          <FiArrowLeft size={20} />
          <span className="font-medium">Back to Consultants</span>
        </Button>
      </Link>

      {/* Header Section */}
      <div className="text-center mb-6">
        <h1 className="text-3xl font-semibold text-gray-800">📅 Book an Appointment</h1>
        <p className="text-gray-600 mt-2">Select a time slot to schedule your appointment.</p>
      </div>

      {/* Appointment Booking Component */}
      <div className="bg-gray-100 p-5 rounded-lg shadow-sm">
        <AppointmentBooking listingId={consultantId} type={"consultant"} />
      </div>
    </div>
  );
};

export default AppointmentBookingCPage;
````

## File: Frontend/src/app/globals.css
````css
@tailwind base;
@tailwind components;
@tailwind utilities;

body {
  font-family: Arial, Helvetica, sans-serif;
}

@layer base {
  :root {
    --background: 0 0% 100%;
    --foreground: 240 10% 3.9%;
    --card: 0 0% 100%;
    --card-foreground: 240 10% 3.9%;
    --popover: 0 0% 100%;
    --popover-foreground: 240 10% 3.9%;
    --primary: 240 5.9% 10%;
    --primary-foreground: 0 0% 98%;
    --secondary: 240 4.8% 95.9%;
    --secondary-foreground: 240 5.9% 10%;
    --muted: 240 4.8% 95.9%;
    --muted-foreground: 240 3.8% 46.1%;
    --accent: 240 4.8% 95.9%;
    --accent-foreground: 240 5.9% 10%;
    --destructive: 0 84.2% 60.2%;
    --destructive-foreground: 0 0% 98%;
    --border: 240 5.9% 90%;
    --input: 240 5.9% 90%;
    --ring: 240 10% 3.9%;
    --chart-1: 12 76% 61%;
    --chart-2: 173 58% 39%;
    --chart-3: 197 37% 24%;
    --chart-4: 43 74% 66%;
    --chart-5: 27 87% 67%;
    --radius: 0.5rem;
  }
  .dark {
    --background: 240 10% 3.9%;
    --foreground: 0 0% 98%;
    --card: 240 10% 3.9%;
    --card-foreground: 0 0% 98%;
    --popover: 240 10% 3.9%;
    --popover-foreground: 0 0% 98%;
    --primary: 0 0% 98%;
    --primary-foreground: 240 5.9% 10%;
    --secondary: 240 3.7% 15.9%;
    --secondary-foreground: 0 0% 98%;
    --muted: 240 3.7% 15.9%;
    --muted-foreground: 240 5% 64.9%;
    --accent: 240 3.7% 15.9%;
    --accent-foreground: 0 0% 98%;
    --destructive: 0 62.8% 30.6%;
    --destructive-foreground: 0 0% 98%;
    --border: 240 3.7% 15.9%;
    --input: 240 3.7% 15.9%;
    --ring: 240 4.9% 83.9%;
    --chart-1: 220 70% 50%;
    --chart-2: 160 60% 45%;
    --chart-3: 30 80% 55%;
    --chart-4: 280 65% 60%;
    --chart-5: 340 75% 55%;
  }
}

@layer base {
  * {
    @apply border-border;
  }
  body {
    @apply bg-background text-foreground;
  }
}
````

## File: Frontend/src/app/layout.tsx
````typescript
import type { Metadata } from "next";
import { Poppins } from "next/font/google";
import "./globals.css";
//import { ThemeProvider } from "@/components/providers/theme-provider";
import "slick-carousel/slick/slick.css";
import "slick-carousel/slick/slick-theme.css";
// import Header from "@/components/Header";

const poppins = Poppins({
  variable: "--font-poppins",
  subsets: [],
  weight: "400",
});

export const metadata: Metadata = {
  title: "ImmiGrow",
  description: "ImmiGrow",
  icons: {
    icon: "/logo.png",
  },
};

export default function RootLayout({
  children,
}: Readonly<{
  children: React.ReactNode;
}>) {
  return (
    <html lang="en" suppressHydrationWarning>
      <body
        className={`${poppins.variable} antialiased overscroll-y-none overscroll-none`}
      >
        {/* <ThemeProvider
          attribute="class"
          defaultTheme="system"
          enableSystem
          disableTransitionOnChange
        > */}
        {children}
        {/* </ThemeProvider> */}
      </body>
    </html>
  );
}
````

## File: Frontend/src/app/page.tsx
````typescript
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import { Button } from "@/components/ui/button";
import {
  Card,
  CardContent,
  CardDescription,
  CardHeader,
  CardTitle,
} from "@/components/ui/card";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import {
  ArrowRight,
  Building,
  Car,
  CheckCircle,
  ChevronRight,
  Globe,
  GraduationCap,
  Home,
  MessageSquare,
  Star,
  Users,
} from "lucide-react";
import Image from "next/image";
import Link from "next/link";

export default function LandingPage() {
  return (
    <div className="flex flex-col min-h-screen min-w-full  bg-background">
      {/* Header */}
      <Header />
      <main className="flex-1">
        {/* Hero Section */}
        <section className="relative overflow-hidden bg-white py-20 md:py-12">
          <div className="absolute inset-0 bg-gradient-to-br from-blue-50 to-white z-0"></div>
          <div className="container relative z-10 mx-auto">
            <div className="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
              <div className="flex m-3 flex-col gap-6">
                <h1 className="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight">
                  Your New Life{" "}
                  <span className="text-blue-500">Starts Here</span>
                </h1>
                <p className="text-xl text-gray-600">
                  AI-powered help for housing, cars, and immigration support —
                  all in one place.
                </p>
                <div className="flex flex-col sm:flex-row gap-4 mt-4">
                  <Link href={"/signup"}>
                    <Button size="lg" className="bg-blue-500 hover:bg-blue-600">
                      Start Planning
                      <ArrowRight className="ml-2 h-4 w-4" />
                    </Button>
                  </Link>
                  <Link href="#how-it-works">
                    <Button size="lg" variant="outline">
                      How It Works
                    </Button>
                  </Link>
                </div>
              </div>
              <div className="relative h-[600px] w-full ">
                <Image
                  src="/landing-1.png"
                  alt="ImmiGrow Hero Image"
                  fill
                  // className="object-cover"
                  priority
                />
                {/* <div className="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent"></div> */}
              </div>
            </div>
          </div>
        </section>

        {/* Platform Overview */}
        <section id="about" className="py-20 bg-white">
          <div className="container mx-auto">
            <div className="text-center mb-16">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                All-in-One Platform for New Immigrants
              </h2>
              <p className="text-xl text-gray-600 max-w-3xl mx-auto">
                Everything you need to start your new life in one place, powered
                by AI.
              </p>
            </div>

            <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
              <Card className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full">
                <CardHeader className="pb-2">
                  <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mb-4">
                    <Home className="h-6 w-6 text-blue-500" />
                  </div>
                  <CardTitle>Housing</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-base">
                    Verified rentals across top cities with virtual tours and
                    trusted landlords.
                  </CardDescription>
                </CardContent>
              </Card>

              <Card className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full">
                <CardHeader className="pb-2">
                  <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mb-4">
                    <Car className="h-6 w-6 text-blue-500" />
                  </div>
                  <CardTitle>Cars</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-base">
                    New & used cars with insurance options tailored for
                    newcomers.
                  </CardDescription>
                </CardContent>
              </Card>

              <Card className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full">
                <CardHeader className="pb-2">
                  <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mb-4">
                    <MessageSquare className="h-6 w-6 text-blue-500" />
                  </div>
                  <CardTitle>Consultants</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-base">
                    Trusted immigration consultants with verified credentials
                    and reviews.
                  </CardDescription>
                </CardContent>
              </Card>

              <Card className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full">
                <CardHeader className="pb-2">
                  <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center mb-4">
                    <Globe className="h-6 w-6 text-blue-500" />
                  </div>
                  <CardTitle>Smart Planner</CardTitle>
                </CardHeader>
                <CardContent>
                  <CardDescription className="text-base">
                    AI-powered immigration guidance customized to your unique
                    situation.
                  </CardDescription>
                </CardContent>
              </Card>
            </div>
          </div>
        </section>

        {/* How It Works */}
        <section id="how-it-works" className="py-20 bg-gray-50">
          <div className="container mx-auto">
            <div className="text-center mb-16">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                How ImmiGrow Works
              </h2>
              <p className="text-xl text-gray-600 max-w-3xl mx-auto">
                Our AI-powered platform simplifies your immigration journey in
                three easy steps.
              </p>
            </div>

            <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
              {[
                {
                  number: "01",
                  title: "Tell Us About Your Move",
                  description:
                    "Where, when, and why you're immigrating. We'll customize everything to your needs.",
                  icon: Globe,
                },
                {
                  number: "02",
                  title: "Get Smart Matches Instantly",
                  description:
                    "AI finds you the right homes, cars, and consultants based on your preferences.",
                  icon: CheckCircle,
                },
                {
                  number: "03",
                  title: "Connect, Book, and Arrive Ready",
                  description:
                    "No stress. No scams. Just a smooth transition to your new home.",
                  icon: Home,
                },
              ].map((step, index) => (
                <div
                  key={index}
                  className="relative flex flex-col items-center text-center p-6"
                >
                  <div className="w-16 h-16 rounded-full bg-blue-500 text-white flex items-center justify-center text-2xl font-bold mb-6">
                    {step.number}
                  </div>
                  <h3 className="text-xl font-bold mb-3">{step.title}</h3>
                  <p className="text-gray-600">{step.description}</p>

                  {index < 2 && (
                    <div className="hidden md:block absolute top-1/4 right-0 transform translate-x-1/2">
                      <ChevronRight className="h-8 w-8 text-blue-300" />
                    </div>
                  )}
                </div>
              ))}
            </div>
          </div>
        </section>

        {/* Who It's For */}
        <section id="who-its-for" className="py-20 bg-white">
          <div className="container mx-auto">
            <div className="text-center mb-16">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                Built for Every Immigrant Journey
              </h2>
              <p className="text-xl text-gray-600 max-w-3xl mx-auto">
                No matter your situation, ImmiGrow has the tools and resources
                you need.
              </p>
            </div>

            <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
              {[
                {
                  title: "International Students",
                  description:
                    "Find student housing, affordable cars, and visa support.",
                  icon: GraduationCap,
                  color: "bg-blue-100",
                },
                {
                  title: "Skilled Workers",
                  description:
                    "Professional relocation support for you and your family.",
                  icon: Building,
                  color: "bg-purple-100",
                },
                {
                  title: "Families",
                  description:
                    "Family-friendly homes, safe vehicles, and community connections.",
                  icon: Users,
                  color: "bg-orange-100",
                },
                {
                  title: "Realtors & Car Dealers",
                  description:
                    "Connect with newcomers looking for your services.",
                  icon: Home,
                  color: "bg-blue-100",
                },
              ].map((segment, index) => (
                <Card
                  key={index}
                  className="border-none shadow-lg hover:shadow-xl transition-shadow duration-300 h-full"
                >
                  <CardHeader className="pb-2">
                    <div
                      className={`w-12 h-12 rounded-full ${segment.color} flex items-center justify-center mb-4`}
                    >
                      <segment.icon className="h-6 w-6 text-blue-500" />
                    </div>
                    <CardTitle>{segment.title}</CardTitle>
                  </CardHeader>
                  <CardContent className="space-y-4">
                    <CardDescription className="text-base">
                      {segment.description}
                    </CardDescription>
                    <Button
                      variant="outline"
                      size="sm"
                      className="text-blue-500 border-blue-500 hover:bg-blue-50"
                    >
                      Get Started
                    </Button>
                  </CardContent>
                </Card>
              ))}
            </div>
          </div>
        </section>

        {/* Testimonials */}
        <section id="testimonials" className="py-20 bg-gray-50">
          <div className="container mx-auto">
            <div className="text-center mb-16">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                Trusted by Thousands Worldwide
              </h2>
              <p className="text-xl text-gray-600 max-w-3xl mx-auto">
                Hear from people who&apos;ve successfully started their new
                lives with ImmiGrow.
              </p>
            </div>

            <div className="grid grid-cols-1 md:grid-cols-3 gap-8 mb-12">
              {[
                {
                  name: "Sarah Chen",
                  location: "From China to Canada",
                  quote:
                    "ImmiGrow helped me find a perfect apartment and a reliable car within days of arriving. The consultant they matched me with made my visa process so much easier.",
                  rating: 5,
                },
                {
                  name: "Miguel Rodriguez",
                  location: "From Mexico to USA",
                  quote:
                    "As a student, I was worried about finding affordable housing. ImmiGrow not only found me a great place but also connected me with other students from my country.",
                  rating: 5,
                },
                {
                  name: "Priya Sharma",
                  location: "From India to Australia",
                  quote:
                    "Moving with my family was stressful until we found ImmiGrow. Their AI recommendations were spot-on for our needs, and we felt at home right away.",
                  rating: 4,
                },
              ].map((testimonial, index) => (
                <Card key={index} className="border-none shadow-lg h-full">
                  <CardContent className="pt-6">
                    <div className="flex items-center mb-4">
                      {Array(testimonial.rating)
                        .fill(0)
                        .map((_, i) => (
                          <Star
                            key={i}
                            className="h-5 w-5 fill-yellow-400 text-yellow-400"
                          />
                        ))}
                    </div>
                    <p className="text-gray-700 mb-6 italic">
                      {testimonial.quote}
                    </p>
                    <div className="flex items-center gap-4">
                      <div className="w-12 h-12 rounded-full bg-blue-100 flex items-center justify-center">
                        <span className="text-blue-500 font-bold">
                          {testimonial.name
                            .split(" ")
                            .map((n) => n[0])
                            .join("")}
                        </span>
                      </div>
                      <div>
                        <p className="font-medium">{testimonial.name}</p>
                        <p className="text-sm text-gray-500">
                          {testimonial.location}
                        </p>
                      </div>
                    </div>
                  </CardContent>
                </Card>
              ))}
            </div>

            <div className="flex justify-center gap-12 flex-wrap">
              <div className="text-center">
                <p className="text-4xl font-bold text-blue-500">5,000+</p>
                <p className="text-gray-600">Users Onboarded</p>
              </div>
              <div className="text-center">
                <p className="text-4xl font-bold text-blue-500">12+</p>
                <p className="text-gray-600">Countries Served</p>
              </div>
              <div className="text-center">
                <p className="text-4xl font-bold text-blue-500">4.9/5</p>
                <p className="text-gray-600">Average Rating</p>
              </div>
            </div>
          </div>
        </section>

        {/* CTA Banner */}
        <section className="py-16 bg-blue-500 text-white">
          <div className="container mx-auto">
            <div className="max-w-4xl mx-auto text-center">
              <h2 className="text-3xl md:text-4xl font-bold mb-4">
                Let&apos;s Plan Your Move - Together
              </h2>
              <p className="text-xl mb-8">
                Takes less than 2 minutes to get matched with the perfect
                housing, transportation, and support.
              </p>
              <Link href={"/signup"}>
                <Button
                  size="lg"
                  className="bg-white text-blue-500 hover:bg-gray-100"
                >
                  Start Now — It&apos;s Free
                  <ArrowRight className="ml-2 h-4 w-4" />
                </Button>
              </Link>
            </div>
          </div>
        </section>

        {/* Contact Form */}
        <section id="contact" className="py-20 m-4 bg-white">
          <div className="container mx-auto">
            <div className="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
              <div>
                <h2 className="text-3xl md:text-4xl font-bold mb-4">
                  Have Questions? Reach Out!
                </h2>
                <p className="text-xl text-gray-600 mb-8">
                  Our team is here to help you with any questions about your
                  immigration journey.
                </p>

                <form className="space-y-6">
                  <div className="space-y-2">
                    <label htmlFor="name" className="text-sm font-medium">
                      Name
                    </label>
                    <Input id="name" placeholder="Your name" />
                  </div>

                  <div className="space-y-2">
                    <label htmlFor="email" className="text-sm font-medium">
                      Email
                    </label>
                    <Input
                      id="email"
                      type="email"
                      placeholder="your.email@example.com"
                    />
                  </div>

                  <div className="space-y-2">
                    <label htmlFor="message" className="text-sm font-medium">
                      Message
                    </label>
                    <Textarea
                      id="message"
                      placeholder="How can we help you?"
                      rows={4}
                    />
                  </div>

                  <Button className="w-full bg-blue-500 hover:bg-blue-600">
                    Send Message
                  </Button>
                </form>
              </div>

              <div className="relative h-[500px] w-full ">
                <Image
                  src="/landing-2.jpg"
                  alt="Contact ImmiGrow"
                  fill
                  className="object-cover"
                />
                {/* <div className="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent"></div> */}
              </div>
            </div>
          </div>
        </section>
      </main>
      {/* Footer */}
      <Footer />
    </div>
  );
}
````

## File: Frontend/src/components/availability/AppointmentBooking.tsx
````typescript
import { useState, useEffect } from "react";
import { Button } from "@/components/ui/button";
import { CalendarClock, Clock, CheckCircle } from "lucide-react";

interface Availability {
  id: string;
  startTime: string;
  endTime: string;
  status: string;
}

interface AppointmentBookingProps {
  listingId: string;
  type: "car" | "house" | "consultant";
}

const AppointmentBooking: React.FC<AppointmentBookingProps> = ({
  listingId,
  type,
}) => {
  const [availability, setAvailability] = useState<Availability[]>([]);
  const [loading, setLoading] = useState(false);
  const [selectedSlot, setSelectedSlot] = useState<string | null>(null);
  const [error, setError] = useState("");
  const [authToken, setAuthToken] = useState<string | null>(null);
  const [isAppointmentBooked, setIsAppointmentBooked] = useState<string | null>(
    null
  );

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // ✅ Convert UTC to User's Timezone for Display
  const formatToUserTimezone = (utcDate: string) => {
    return new Intl.DateTimeFormat("en-US", {
      year: "numeric",
      month: "2-digit",
      day: "2-digit",
      hour: "2-digit",
      minute: "2-digit",
      hour12: true,
    }).format(new Date(utcDate));
  };

  // ✅ Fetch Authentication Token Once
  useEffect(() => {
    const fetchToken = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        setAuthToken(tokenData.token);
      } catch (error) {
        setError("Authentication error. Please try again.");
      }
    };

    fetchToken();
  }, []);

  // ✅ Fetch Availability Slots
  const fetchAvailability = async () => {
    if (!authToken) return;

    setLoading(true);
    setError("");

    if (type === "consultant") {
      try {
        const response = await fetch(
          `${endpoint}api/protected/availability/consultant-availability/${listingId}`,
          {
            method: "GET",
            headers: { Authorization: `Bearer ${authToken}` },
          }
        );

        if (!response.ok) throw new Error("Failed to fetch availability");

        const data: Availability[] = await response.json();
        setAvailability(data);
      } catch (error) {
        setError("Error fetching availability. Please try again.");
      } finally {
        setLoading(false);
      }
    } else {
      try {
        const response = await fetch(
          `${endpoint}api/protected/availability/express-interest?type=${type}&listingId=${listingId}`,
          {
            method: "GET",
            headers: { Authorization: `Bearer ${authToken}` },
          }
        );

        if (!response.ok) throw new Error("Failed to fetch availability");

        const data: Availability[] = await response.json();
        setAvailability(data);
      } catch (error) {
        setError("Error fetching availability. Please try again.");
      } finally {
        setLoading(false);
      }
    }
  };

  useEffect(() => {
    if (authToken) fetchAvailability();
  }, [authToken, listingId, type]);

  // ✅ Handle Booking Appointment
  const handleBookAppointment = async (
    availabilityId: string,
    listingId: string
  ) => {
    if (!authToken) return;

    try {
      setSelectedSlot(availabilityId);

      const response = await fetch(
        `${endpoint}api/protected/appointment/schedule`,
        {
          method: "POST",
          headers: {
            "Content-Type": "application/json",
            Authorization: `Bearer ${authToken}`,
          },
          body: JSON.stringify({
            listingId: parseInt(listingId),
            availabilityId: parseInt(availabilityId),
          }),
        }
      );

      const data = await response.json();

      if (
        data.error ===
        "Google Calendar access required. Please connect your Google account."
      ) {
        alert("Google Calendar access required. Redirecting...");
        window.open(data.connectUrl, "_blank"); // Open Google OAuth link
      } else if (data.appointment) {
        alert("✅ Appointment Scheduled! Check your Google Calendar.");
        setIsAppointmentBooked(availabilityId);
      } else {
        alert("Failed to schedule appointment.");
      }
    } catch (error) {
      console.error("Error scheduling appointment:", error);
      alert("Error scheduling event.");
    }
  };

  return (
    <div className="mx-auto p-6">
      {loading ? (
        <p className="text-center text-gray-600">Loading...</p>
      ) : error ? (
        <p className="text-red-500 text-center">{error}</p>
      ) : availability.length === 0 ? (
        <p className="text-gray-500 text-center">
          No available slots at the moment.
        </p>
      ) : (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {availability.map((slot) => (
            <div
              key={slot.id}
              className={`p-5 border rounded-lg shadow-md flex flex-col ${
                selectedSlot === slot.id ? "bg-blue-100" : "bg-white"
              } transition-transform hover:scale-105`}
            >
              <div className="flex items-center space-x-3 mb-3">
                <CalendarClock className="w-6 h-6 text-gray-600" />
                <h3 className="text-lg font-semibold text-gray-800">
                  Time Slot
                </h3>
              </div>

              <div className="bg-gray-100 p-4 rounded-lg mb-3">
                <div className="flex items-center space-x-2">
                  <Clock className="w-5 h-5 text-blue-600" />
                  <p className="text-gray-900 font-semibold">Start:</p>
                  <p className="text-gray-700">
                    {formatToUserTimezone(slot.startTime)}
                  </p>
                </div>
                <div className="flex items-center space-x-2 mt-2">
                  <Clock className="w-5 h-5 text-red-600" />
                  <p className="text-gray-900 font-semibold">End:</p>
                  <p className="text-gray-700">
                    {formatToUserTimezone(slot.endTime)}
                  </p>
                </div>
              </div>

              <Button
                className="bg-blue-600 hover:bg-blue-500 text-white px-4 py-2 rounded-lg flex items-center justify-center"
                onClick={() => handleBookAppointment(slot.id, listingId)}
                disabled={isAppointmentBooked === slot.id}
              >
                {isAppointmentBooked === slot.id ? (
                  <>
                    <CheckCircle className="w-5 h-5 mr-2" />
                    Appointment Booked
                  </>
                ) : (
                  "Book Appointment"
                )}
              </Button>
            </div>
          ))}
        </div>
      )}
    </div>
  );
};

export default AppointmentBooking;
````

## File: Frontend/src/components/availability/AvailabilityForm.tsx
````typescript
import { useState, useEffect } from "react";
import { Button } from "@/components/ui/button";

interface AvailabilityFormProps {
  initialData?: { id: string; startTime: string; endTime: string };
  refreshSlots: () => void;
  onClose: () => void;
}

const AvailabilityForm: React.FC<AvailabilityFormProps> = ({
  initialData,
  refreshSlots,
  onClose,
}) => {
  const [formData, setFormData] = useState({
    startTime: "",
    endTime: "",
  });

  const [error, setError] = useState("");
  const [loading, setLoading] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  // **UseEffect to load initial data properly when editing**
  useEffect(() => {
    if (initialData) {
      setFormData({
        startTime: initialData.startTime || "",
        endTime: initialData.endTime || "",
      });
    }
  }, [initialData]); // ✅ Triggers when initialData changes

  const handleChange = (e: React.ChangeEvent<HTMLInputElement>) => {
    setFormData((prev) => ({
      ...prev,
      [e.target.name]: e.target.value,
    }));
  };

  const handleSubmit = async (e: React.FormEvent) => {
    e.preventDefault();

    if (!formData.startTime || !formData.endTime) {
      setError("Both start time and end time are required.");
      return;
    }

    const start = new Date(formData.startTime);
    const end = new Date(formData.endTime);

    if (start >= end) {
      setError("Start time must be before end time.");
      return;
    }

    const duration = (end.getTime() - start.getTime()) / (1000 * 60); // Duration in minutes

    if (duration > 60) {
      setError("Slots cannot be longer than 1 hour.");
      return;
    }

    setError("");
    setLoading(true);

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;

      const url = initialData
        ? `${endpoint}api/protected/availability/update/${initialData.id}`
        : `${endpoint}api/protected/availability/add`;
      const method = initialData ? "PUT" : "POST";

      const response = await fetch(url, {
        method,
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
        body: JSON.stringify({
          startTime: formData.startTime,
          endTime: formData.endTime,
          status: "Available",
        }),
      });

      if (!response.ok) throw new Error("Failed to save availability");

      refreshSlots(); // Refresh the slots list
      onClose(); // Close form
    } catch (error) {
      setError("Error saving availability. Please try again." + error);
    } finally {
      setLoading(false);
    }
  };

  return (
    <div className="max-w-md mx-auto p-6 border rounded-lg shadow-lg mb-4 ">
      <h2 className="text-2xl font-semibold text-gray-800 mb-4">
        {initialData ? "Edit Availability" : "Add Availability"}
      </h2>

      {error && <p className="text-red-500  p-2 rounded mb-2">{error}</p>}

      <form onSubmit={handleSubmit} className="space-y-4">
        <div>
          <label className="block text-sm font-medium text-gray-700">
            Start Time
          </label>
          <input
            type="datetime-local"
            name="startTime"
            value={formData.startTime}
            onChange={handleChange}
            className="w-full p-2 border rounded-md focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
            required
          />
        </div>

        <div>
          <label className="block text-sm font-medium text-gray-700">
            End Time
          </label>
          <input
            type="datetime-local"
            name="endTime"
            value={formData.endTime}
            onChange={handleChange}
            className="w-full p-2 border rounded-md focus:ring-2 focus:ring-blue-500 focus:border-blue-500"
            required
          />
        </div>

        <div className="flex justify-between">
          <Button
            type="submit"
            className="bg-blue-600 hover:bg-blue-500"
            disabled={loading}
          >
            {loading ? "Saving..." : initialData ? "Update" : "Submit"}
          </Button>
          <Button
            className="bg-gray-400 hover:bg-gray-300"
            onClick={onClose}
            disabled={loading}
          >
            Cancel
          </Button>
        </div>
      </form>
    </div>
  );
};

export default AvailabilityForm;
````

## File: Frontend/src/components/availability/AvailabilityPage.tsx
````typescript
import { useState, useEffect } from "react";
import { Button } from "@/components/ui/button";
import { Pencil, Trash, Plus, CalendarClock, Clock } from "lucide-react";
import AvailabilityForm from "./AvailabilityForm";

interface Availability {
  id: string;
  startTime: string;
  endTime: string;
}

const AvailabilityPage: React.FC = () => {
  const [slots, setSlots] = useState<Availability[]>([]);
  const [showForm, setShowForm] = useState(false);
  const [editSlot, setEditSlot] = useState<Availability | null>(null);
  const [loading, setLoading] = useState(false);

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  const fetchSlots = async () => {
    setLoading(true);
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;
      const response = await fetch(
        `${endpoint}api/protected/availability/byId`,
        {
          method: "GET",
          headers: { Authorization: `Bearer ${token}` },
        }
      );

      if (!response.ok) throw new Error("Failed to fetch slots");

      const data: Availability[] = await response.json();

      if (data.length == 0) {
        setSlots([]);
      } else {
        setSlots(data);
      }
    } catch (error) {
      console.error(error);
    } finally {
      setLoading(false);
    }
  };

  useEffect(() => {
    fetchSlots();
  }, []);

  const handleDelete = async (id: string) => {
    if (!confirm("Are you sure you want to delete this slot?")) return;

    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;
      const response = await fetch(
        `${endpoint}api/protected/availability/delete/${id}`,
        {
          method: "DELETE",
          headers: {
            Authorization: `Bearer ${token}`,
          },
        }
      );
      if (!response.ok) throw new Error("Failed to delete");

      setSlots(slots.filter((slot) => slot.id !== id));
    } catch (error) {
      console.error(error);
    }
  };
  const formatToDateTimeLocal = (utcDate: string) => {
    if (!utcDate) return "";

    const date = new Date(utcDate);

    // Get user's local time components
    const year = date.getFullYear();
    const month = String(date.getMonth() + 1).padStart(2, "0"); // Months are 0-based
    const day = String(date.getDate()).padStart(2, "0");
    const hours = String(date.getHours()).padStart(2, "0");
    const minutes = String(date.getMinutes()).padStart(2, "0");

    return `${year}-${month}-${day}T${hours}:${minutes}`; // Format: "YYYY-MM-DDTHH:MM"
  };

  const handleEdit = (slot: Availability) => {
    const slotLocal = { ...slot };
    slotLocal.startTime = formatToDateTimeLocal(slot.startTime);
    slotLocal.endTime = formatToDateTimeLocal(slot.endTime);

    setEditSlot(slotLocal);
    setShowForm(true);
  };

  return (
    <div className=" mx-auto p-6">
      <div className="flex justify-between items-center mb-6">
        <h2 className="text-2xl font-bold mb-6 mt-4">Availability Slots</h2>
        <Button
          className="bg-blue-600 hover:bg-blue-500 flex items-center px-4 py-2 text-white font-medium rounded-lg shadow-md"
          onClick={() => {
            setShowForm(true);
            setEditSlot(null);
          }}
        >
          <Plus className="w-5 h-5 mr-2" /> Add Slots
        </Button>
      </div>

      {showForm && (
        <AvailabilityForm
          initialData={editSlot}
          refreshSlots={fetchSlots}
          onClose={() => setShowForm(false)}
        />
      )}

      {loading ? (
        <p className="text-center text-gray-600">Loading...</p>
      ) : slots.length === 0 ? (
        <p className="text-gray-500 text-center">No slots added yet.</p>
      ) : (
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          {slots.map((slot) => (
            <div
              key={slot.id}
              className="p-5 border border-gray-200 rounded-xl shadow-md bg-white flex flex-col transition-transform hover:scale-105 hover:shadow-lg"
            >
              <div className="flex items-center space-x-3 mb-2">
                <CalendarClock className="w-6 h-6 text-gray-600" />
                <h3 className="text-lg font-semibold text-gray-800">
                  Availability Slot
                </h3>
              </div>

              <div className="bg-gray-100 p-4 rounded-lg mb-3 flex flex-col">
                <div className="flex items-center space-x-2">
                  <Clock className="w-5 h-5 text-blue-600" />
                  <p className="text-gray-900 font-semibold">Start:</p>
                  <p className="text-gray-700">
                    {slot.startTime
                      ? new Date(slot.startTime).toLocaleString()
                      : "Invalid Date"}
                  </p>
                </div>
                <div className="flex items-center space-x-2 mt-2">
                  <Clock className="w-5 h-5 text-red-600" />
                  <p className="text-gray-900 font-semibold">End:</p>
                  <p className="text-gray-700">
                    {" "}
                    {slot.endTime
                      ? new Date(slot.endTime).toLocaleString()
                      : "Invalid Date"}
                  </p>
                </div>
              </div>

              <div className="flex justify-between items-center">
                <span className="text-blue-600 font-semibold bg-blue-100 px-3 py-1 rounded-full text-sm">
                  ✅ Available
                </span>
                <div className="flex gap-2">
                  <Button
                    className="bg-blue-500 hover:bg-blue-400 p-2 rounded-lg"
                    size="icon"
                    onClick={() => handleEdit(slot)}
                  >
                    <Pencil className="w-5 h-5 text-white" />
                  </Button>
                  <Button
                    className="bg-red-500 hover:bg-red-400 p-2 rounded-lg"
                    size="icon"
                    onClick={() => handleDelete(slot.id)}
                  >
                    <Trash className="w-5 h-5 text-white" />
                  </Button>
                </div>
              </div>
            </div>
          ))}
        </div>
      )}
    </div>
  );
};

export default AvailabilityPage;
````

## File: Frontend/src/components/availability/BookingTable.tsx
````typescript
import React, { useEffect, useState } from "react";
import { Button } from "@/components/ui/button";
import {
  Dialog,
  DialogContent,
  DialogHeader,
  DialogTitle,
  DialogClose,
} from "@/components/ui/dialog";

interface Booking {
  id: number;
  userId: number;
  listingId: number;
  startDate: string;
  endDate: string;
  status: string;
  meetLink?: string;
  createdAt: string;
  listing?: {
    id: number;
    title?: string;
    price?: string;
    location?: string;
    make?: string;
    model?: string;
    year?: number;
  };
}

interface User {
  id: number;
  fullName: string;
  email: string;
  phoneNo: string;
  role: string;
}

const BookingTable = () => {
  const [houseBookings, setHouseBookings] = useState<Booking[]>([]);
  const [carBookings, setCarBookings] = useState<Booking[]>([]);
  const [icBookings, setIcBookings] = useState<Booking[]>([]);
  const [loading, setLoading] = useState(true);
  const [modalData, setModalData] = useState<{
    type: "user" | "listing";
    data: any;
  } | null>(null);
  let id = 1;

  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  useEffect(() => {
    const fetchBookings = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok)
          throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;

        const response = await fetch(
          `${endpoint}api/protected/appointment/user-info`,
          {
            method: "GET",
            headers: { Authorization: `Bearer ${token}` },
          }
        );

        const data = await response.json();
        if (data.success) {
          setHouseBookings(data.houseBookings || []);
          setCarBookings(data.carBookings || []);
          setIcBookings(data.icBookings || []);
          id = 1;
        }
      } catch (error) {
        console.error("Error fetching bookings:", error);
      } finally {
        setLoading(false);
      }
    };

    fetchBookings();
  }, []);

  const markAsComplete = async (
    id: number,
    type: "house" | "car" | "consultant"
  ) => {
    try {
      const tokenResponse = await fetch(`${endpoint}auth/token`, {
        credentials: "include",
      });

      if (!tokenResponse.ok) {
        throw new Error("Failed to get authentication token");
      }

      const tokenData = await tokenResponse.json();
      const token = tokenData.token;
      const res = await fetch(`${endpoint}api/protected/appointment/complete`, {
        method: "PUT",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
        body: JSON.stringify({ id, type }),
      });

      if (res.ok) {
        id = 1;
        window.location.reload();
      }
    } catch (error) {
      console.error("Error updating booking status:", error);
    }
  };

  if (loading) return <p>Loading...</p>;

  return (
    <div className="p-4">
      <h2 className="text-xl font-semibold mb-4">Booking Details</h2>

      {/* House Bookings */}

      {houseBookings.length > 0 && (
        <div>
          <table className="w-full border-collapse border border-gray-300">
            <thead>
              <tr className="bg-gray-100">
                <th className="border p-2">ID</th>
                <th className="border p-2">User</th>
                <th className="border p-2">Listing</th>
                <th className="border p-2">Start Date</th>
                <th className="border p-2">End Date</th>
                <th className="border p-2">Status</th>
                <th className="border p-2">Actions</th>
              </tr>
            </thead>
            <tbody>
              {houseBookings.map((booking) => (
                <tr key={booking.id} className="border">
                  <td className="border p-2 text-center">{id++}</td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "user", data: booking.user })
                      }
                    >
                      View User
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "listing", data: booking.listing })
                      }
                    >
                      View Listing
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.startDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.endDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">{booking.status}</td>
                  <td className="border p-2 text-center">
                    {booking.status !== "completed" && (
                      <Button
                        onClick={() => markAsComplete(booking.id, "house")}
                        className="bg-blue-600 hover:bg-blue-500"
                      >
                        Mark as Complete
                      </Button>
                    )}
                  </td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      )}
      {carBookings.length > 0 && (
        <div>
          <table className="w-full border-collapse border border-gray-300">
            <thead>
              <tr className="bg-gray-100">
                <th className="border p-2">ID</th>
                <th className="border p-2">User</th>
                <th className="border p-2">Listing</th>
                <th className="border p-2">Start Date</th>
                <th className="border p-2">End Date</th>
                <th className="border p-2">Status</th>
                <th className="border p-2">Actions</th>
              </tr>
            </thead>
            <tbody>
              {carBookings.map((booking) => (
                <tr key={booking.id} className="border">
                  <td className="border p-2 text-center">{id++}</td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "user", data: booking.user })
                      }
                    >
                      View User
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "listing", data: booking.listing })
                      }
                    >
                      View Listing
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.startDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.endDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">{booking.status}</td>
                  <td className="border p-2 text-center">
                    {booking.status !== "completed" && (
                      <Button
                        onClick={() => markAsComplete(booking.id, "car")}
                        className="bg-blue-600 hover:bg-blue-500"
                      >
                        Mark as Complete
                      </Button>
                    )}
                  </td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      )}

      {icBookings.length > 0 && (
        <div>
          <table className="w-full border-collapse border border-gray-300">
            <thead>
              <tr className="bg-gray-100">
                <th className="border p-2">ID</th>
                <th className="border p-2">User</th>
                <th className="border p-2">Start Date</th>
                <th className="border p-2">End Date</th>
                <th className="border p-2">Status</th>
                <th className="border p-2">Actions</th>
              </tr>
            </thead>
            <tbody>
              {icBookings.map((booking) => (
                <tr key={booking.id} className="border">
                  <td className="border p-2 text-center">{id++}</td>
                  <td className="border p-2 text-center">
                    <Button
                      variant="link"
                      onClick={() =>
                        setModalData({ type: "user", data: booking.user })
                      }
                    >
                      View User
                    </Button>
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.startDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">
                    {new Date(booking.endDate).toLocaleString()}
                  </td>
                  <td className="border p-2 text-center">{booking.status}</td>
                  <td className="border p-2 text-center">
                    {booking.status !== "completed" && (
                      <Button
                        onClick={() => markAsComplete(booking.id, "consultant")}
                        className="bg-blue-600 hover:bg-blue-500"
                      >
                        Mark as Complete
                      </Button>
                    )}
                  </td>
                </tr>
              ))}
            </tbody>
          </table>
        </div>
      )}
      {houseBookings.length === 0 &&
        carBookings.length === 0 &&
        icBookings.length === 0 && (
          <div className="text-center p-4">No bookings found</div>
        )}
      {/* Modal for viewing details */}
      {modalData && (
        <Dialog open={!!modalData} onOpenChange={() => setModalData(null)}>
          <DialogContent>
            <DialogHeader>
              <DialogTitle>
                {modalData.type === "user" ? "User Details" : "Listing Details"}
              </DialogTitle>
            </DialogHeader>
            <div className="p-4 bg-gray-100 rounded">
              {modalData.type === "user" ? (
                <>
                  <p>
                    <strong>Full Name:</strong> {modalData.data.fullName}
                  </p>
                  <p>
                    <strong>Email:</strong> {modalData.data.email}
                  </p>
                  <p>
                    <strong>Phone:</strong> {modalData.data.phoneNo}
                  </p>
                </>
              ) : (
                <>
                  {modalData.data.title && (
                    <p>
                      <strong>Title:</strong> {modalData.data.title}
                    </p>
                  )}
                  {modalData.data.price && (
                    <p>
                      <strong>Price:</strong> {modalData.data.price}
                    </p>
                  )}
                  {modalData.data.location && (
                    <p>
                      <strong>Location:</strong> {modalData.data.location}
                    </p>
                  )}
                  {modalData.data.make && (
                    <p>
                      <strong>Make:</strong> {modalData.data.make}
                    </p>
                  )}
                  {modalData.data.model && (
                    <p>
                      <strong>Model:</strong> {modalData.data.model}
                    </p>
                  )}
                  {modalData.data.year && (
                    <p>
                      <strong>Year:</strong> {modalData.data.year}
                    </p>
                  )}
                </>
              )}
            </div>
            <DialogClose asChild>
              <Button className="mt-2">Close</Button>
            </DialogClose>
          </DialogContent>
        </Dialog>
      )}
    </div>
  );
};

export default BookingTable;
````

## File: Frontend/src/components/availability/UserBooking.tsx
````typescript
import React, { useEffect, useState } from "react";
import { Button } from "@/components/ui/button";
import { Dialog, DialogContent, DialogHeader, DialogTitle, DialogClose } from "@/components/ui/dialog";
import { Tabs, TabsList, TabsTrigger, TabsContent } from "@/components/ui/tabs";

interface Listing {
  id: number;
  title?: string;
  price?: string;
  location?: string;
  make?: string;
  model?: string;
  year?: number;
}

interface Booking {
  id: number;
  userId: number;
  listingId: number;
  startDate: string;
  endDate: string;
  status: string;
  meetLink?: string;
  createdAt: string;
  listing?: Listing;
  user?: {
    id: number;
    fullName: string;
    email: string;
    phoneNo: string;
  };
}

interface ConsultantBooking {
  id: number;
  consultantId: number;
  startDate: string;
  endDate: string;
  createdAt: string;
  status: string;
  meetLink: string;
  consultant: {
    fullName: string;
    email: string;
    phoneNo: string;
  };
}

interface User {
  id: number;
  fullName: string;
  email: string;
  phoneNo: string;
  role: string;
}

const BookingView = () => {
  const [houseBookings, setHouseBookings] = useState<Booking[]>([]);
  const [carBookings, setCarBookings] = useState<Booking[]>([]);
  const [consultantBookings, setConsultantBookings] = useState<ConsultantBooking[]>([]);
  const [user, setUser] = useState<User | null>(null);
  const [loading, setLoading] = useState(true);
  const [modalData, setModalData] = useState<{ type: "user" | "listing" | "consultant"; data: any } | null>(null);

  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  let id = 0;

  useEffect(() => {
    const fetchBookings = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, { credentials: "include" });
        if (!tokenResponse.ok) throw new Error("Failed to get authentication token");

        const tokenData = await tokenResponse.json();
        const token = tokenData.token;

        // House & Car Bookings
        const response = await fetch(`${endpoint}api/protected/appointment/view-booking`, {
          method: "GET",
          headers: { Authorization: `Bearer ${token}` },
        });
        const data = await response.json();

        if (data.success) {
          setHouseBookings(data.houseBookings || []);
          setCarBookings(data.carBookings || []);
        }

        // Consultant Bookings
        const consultantRes = await fetch(`${endpoint}api/protected/appointment/view-Cbooking`, {
          method: "GET",
          headers: { Authorization: `Bearer ${token}` },
        });
        const consultantData = await consultantRes.json();
        if (Array.isArray(consultantData)) {
          setConsultantBookings(consultantData);
        }

      } catch (error) {
        console.error("Error fetching bookings:", error);
      } finally {
        setLoading(false);
      }
    };

    fetchBookings();
  }, []);

  if (loading) return <p>Loading...</p>;

  return (
    <div className="p-4">
      <h2 className="text-xl font-semibold mb-4">Booking Details</h2>

      <Tabs defaultValue="house">
        <TabsList className="grid w-full grid-cols-3">
          <TabsTrigger value="house">House Bookings</TabsTrigger>
          <TabsTrigger value="car">Car Bookings</TabsTrigger>
          <TabsTrigger value="consultant">Consultant Bookings</TabsTrigger>
        </TabsList>

        <TabsContent value="house">
          {houseBookings.length > 0 ? (
            <TableComponent data={houseBookings} id ={1} type="house" onViewDetails={setModalData} />
          ) : (
            <p>No house bookings found.</p>
          )}
        </TabsContent>

        <TabsContent value="car">
          {carBookings.length > 0 ? (
            <TableComponent data={carBookings}  id ={1}  type="car" onViewDetails={setModalData} />
          ) : (
            <p>No car bookings found.</p>
          )}
        </TabsContent>

        <TabsContent value="consultant">
          {consultantBookings.length > 0 ? (
            <TableComponent data={consultantBookings}  id ={1}  type="consultant" onViewDetails={setModalData} />
          ) : (
            <p>No consultant bookings found.</p>
          )}
        </TabsContent>
      </Tabs>

      {modalData && (
        <Dialog open={!!modalData} onOpenChange={() => setModalData(null)}>
          <DialogContent>
            <DialogHeader>
              <DialogTitle>
                {modalData.type === "user"
                  ? "User Details"
                  : modalData.type === "listing"
                  ? "Listing Details"
                  : "Consultant Details"}
              </DialogTitle>
            </DialogHeader>
            <div className="p-4 bg-gray-100 rounded">
              {modalData.type === "consultant" ? (
                <>
                  <p><strong>Full Name:</strong> {modalData.data.fullName}</p>
                  <p><strong>Email:</strong> {modalData.data.email}</p>
                  <p><strong>Phone:</strong> {modalData.data.phoneNo}</p>
                </>
              ) : modalData.type === "user" ? (
                modalData.data.listing?.landlord || modalData.data.listing?.dealership ? (
                  <>
                    <p><strong>Full Name:</strong> {modalData.data.listing.landlord?.fullName || modalData.data.listing.dealership?.fullName}</p>
                    <p><strong>Email:</strong> {modalData.data.listing.landlord?.email || modalData.data.listing.dealership?.email}</p>
                    <p><strong>Phone:</strong> {modalData.data.listing.landlord?.phoneNo || modalData.data.listing.dealership?.phoneNo}</p>
                  </>
                ) : (
                  <p>No landlord or dealership information available.</p>
                )
              ) : (
                <>
                  {modalData.data.title && <p><strong>Title:</strong> {modalData.data.title}</p>}
                  {modalData.data.price && <p><strong>Price:</strong> {modalData.data.price}</p>}
                  {modalData.data.location && <p><strong>Location:</strong> {modalData.data.location}</p>}
                  {modalData.data.make && <p><strong>Make:</strong> {modalData.data.make}</p>}
                  {modalData.data.model && <p><strong>Model:</strong> {modalData.data.model}</p>}
                  {modalData.data.year && <p><strong>Year:</strong> {modalData.data.year}</p>}
                </>
              )}
            </div>
            <DialogClose asChild>
              <Button className="mt-2">Close</Button>
            </DialogClose>
          </DialogContent>
        </Dialog>
      )}
    </div>
  );
};

const TableComponent = ({
  data,
  type,
  id,
  onViewDetails,
}: {
  data: any[];
  type: "house" | "car" | "consultant";
  id: number,
  onViewDetails: (data: { type: "user" | "listing" | "consultant"; data: any }) => void;
}) => {
  return (
    <table className="w-full border-collapse border border-gray-300">
      <thead>
        <tr className="bg-gray-100">
          <th className="border p-2">ID</th>
          {type === "consultant" ? <th className="border p-2">Consultant</th> : <>
            <th className="border p-2">User</th>
            <th className="border p-2">Listing</th>
          </>}
          <th className="border p-2">Start Date</th>
          <th className="border p-2">End Date</th>
          <th className="border p-2">Status</th>
        </tr>
      </thead>
      <tbody>
        {data.map((booking) => (
          <tr key={booking.id} className="border">
            <td className="border p-2 text-center">{id++}</td>
            {type === "consultant" ? (
              <td className="border p-2 text-center">
                <Button variant="link" onClick={() => onViewDetails({ type: "consultant", data: booking.consultant })}>
                  View Consultant
                </Button>
              </td>
            ) : (
              <>
                <td className="border p-2 text-center">
                  <Button variant="link" onClick={() => onViewDetails({ type: "user", data: booking })}>
                    View User
                  </Button>
                </td>
                <td className="border p-2 text-center">
                  <Button variant="link" onClick={() => onViewDetails({ type: "listing", data: booking.listing })}>
                    View Listing
                  </Button>
                </td>
              </>
            )}
            <td className="border p-2 text-center">{new Date(booking.startDate).toLocaleString()}</td>
            <td className="border p-2 text-center">{new Date(booking.endDate).toLocaleString()}</td>
            <td className="border p-2 text-center">{booking.status}</td>
          </tr>
        ))}
      </tbody>
    </table>
  );
};

export default BookingView;
````

## File: Frontend/src/components/consultant/ConsultantCarousel.tsx
````typescript
"use client";

import React, { useState } from "react";
import { useRouter } from "next/navigation";
import {
  Dialog,
  DialogContent,
  DialogHeader,
  DialogTitle,
} from "@/components/ui/dialog";
import { Button } from "@/components/ui/button";
import { User } from "lucide-react";

const ConsultantCarousel = ({ consultants }) => {
  const [selectedConsultant, setSelectedConsultant] = useState(null);
  const [modalOpen, setModalOpen] = useState(false);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  const router = useRouter();

  const checkIfAnyDateIsFuture = (data) => {
    // Get current UTC time
    const currentTime = new Date();

    // Use Array.some() to stop as soon as a future date is found
    const isFuture = data.some((item) => {
      // Validate if endDate exists and is a valid date
      if (!item.endDate) return false;

      // Convert endDate to a Date object
      const endDateUTC = new Date(item.endDate);

      // Check if endDate is valid and greater than currentTime
      return !isNaN(endDateUTC.getTime()) && endDateUTC > currentTime;
    });

    return isFuture;
  };

  const openModal = (consultant) => {
    setSelectedConsultant(consultant);
    setModalOpen(true);
  };

  const closeModal = () => {
    setSelectedConsultant(null);
    setModalOpen(false);
  };

  if (!consultants || consultants.length === 0) {
    return <p className="text-gray-500">No consultants available.</p>;
  }

  const handleAvailability = async (consultantId: number, type: string) => {
    const tokenResponse = await fetch(`${endpoint}auth/token`, {
      credentials: "include",
    });
    if (!tokenResponse.ok) {
      throw new Error("Failed to get authentication token");
    }
    const tokenData = await tokenResponse.json();
    const token = tokenData?.token;
    const listingId = consultantId;
    const response = await fetch(
      `${endpoint}api/protected/appointment/booking-status?listingId=${listingId}&type=${type}`,
      {
        method: "GET",
        headers: {
          "Content-Type": "application/json",
          Authorization: `Bearer ${token}`,
        },
      }
    );
    if (response.status === 200) {
      const data = await response.json();
      if (checkIfAnyDateIsFuture(data.booking)) {
        alert("You have already booked an appointment with this seller");
      } else {
        alert("Action Pending from Consultant");
      }
    } else {
      router.push(`/dashboard/user/slots/consultant/${consultantId}`);
    }
  };

  return (
    <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
      {consultants.map((consultant) => (
        <div key={consultant.id} className="p-2">
          <div className="rounded-2xl overflow-hidden shadow-md bg-white text-center">
            {/* Top bar with gradient */}
            <div className="relative bg-gradient-to-r from-blue-600 to-blue-400 h-20 flex justify-center items-end rounded-t-2xl">
              {/* User Icon inside circle */}
              <div className="w-16 h-16 rounded-full bg-white flex items-center justify-center shadow-lg -mb-8">
                <User className="w-8 h-8 text-blue-600" />
              </div>
            </div>

            {/* Info below icon */}
            <div className="pt-10 px-4 pb-6">
              <p className="text-sm font-semibold text-blue-600 uppercase tracking-wide">
                {consultant.user?.fullName || "Unknown Consultant"}
              </p>
              <p className="text-sm text-gray-600">
                {consultant.user?.email || "No email provided"}
              </p>
              <p className="text-xs text-gray-500 mt-1 italic">
                {(consultant.servicesOffered || "")
                  .split(",")
                  .map((s) => s.trim())
                  .join(" | ")}
              </p>

              <div className="mt-4 space-y-2">
                <Button
                  className="w-full bg-blue-600 hover:bg-blue-500"
                  onClick={() => openModal(consultant)}
                >
                  View Details
                </Button>

                <Button
                  className="w-full bg-blue-600 hover:bg-blue-500"
                  onClick={() =>
                    handleAvailability(consultant.user.id, "consultant")
                  }
                >
                  View Availability
                </Button>
              </div>
            </div>
          </div>
        </div>
      ))}

      {/* Consultant Details Modal */}
      <Dialog open={modalOpen} onOpenChange={setModalOpen}>
        <DialogContent>
          <DialogHeader>
            <DialogTitle>Consultant Info</DialogTitle>
          </DialogHeader>
          {selectedConsultant && (
            <div className="space-y-2">
              <p>
                <strong>Business Name:</strong>{" "}
                {selectedConsultant.businessName || "N/A"}
              </p>
              <p>
                <strong>Address:</strong>{" "}
                {selectedConsultant.businessAddress || "N/A"}
              </p>
              <p>
                <strong>Experience:</strong>{" "}
                {selectedConsultant.yearsOfExperience || "N/A"} years
              </p>

              <p>
                <strong>Languages:</strong>{" "}
                {selectedConsultant.languagesSpoken || "N/A"}
              </p>
              <p>
                <strong>Website/Social:</strong>{" "}
                {selectedConsultant.websiteOrSocialMedia || "N/A"}
              </p>
              <p>
                <strong>Consultation Fee:</strong>{" "}
                {selectedConsultant.consultationFee
                  ? `$${selectedConsultant.consultationFee}`
                  : "N/A"}
              </p>
            </div>
          )}
        </DialogContent>
      </Dialog>
    </div>
  );
};

export default ConsultantCarousel;
````

## File: Frontend/src/components/consultant/UpcomingMeetings.tsx
````typescript
"use client";

import React, { useEffect, useState } from "react";
import { VideoIcon } from "lucide-react";
import { Button } from "@/components/ui/button";

interface Meeting {
  id: number;
  startDate: string; // already timezone-adjusted by backend
  endDate: string;
  meetLink: string;
  user: {
    fullName: string;
    email: string;
    phoneNo: string;
  };
}

const UpcomingConsultantMeetings = () => {
  const [meetings, setMeetings] = useState<Meeting[]>([]);
  const [loading, setLoading] = useState(true);
  const endpoint = process.env.NEXT_PUBLIC_API_URL;

  useEffect(() => {
    const fetchMeetings = async () => {
      try {
        const tokenResponse = await fetch(`${endpoint}auth/token`, {
          credentials: "include",
        });
        if (!tokenResponse.ok) {
          throw new Error("Failed to get authentication token");
        }
        const tokenData = await tokenResponse.json();
        const token = tokenData?.token;
        const res = await fetch(
          `${endpoint}api/protected/consultants/upcoming`,
          {
            credentials: "include",
            headers: {
              Authorization: `Bearer ${token}`,
            },
          }
        );
        const data = await res.json();

        if (data.success) {
          setMeetings(data.meetings);
        }
      } catch (err) {
        console.error("Failed to fetch upcoming meetings:", err);
      } finally {
        setLoading(false);
      }
    };

    fetchMeetings();
  }, []);

  if (loading) return <p>Loading meetings...</p>;
  if (meetings.length === 0) return <p>No upcoming meetings.</p>;

  return (
    <div className="flex flex-col gap-4">
      {meetings.map((meeting) => (
        <div
          key={meeting.id}
          className="flex flex-row items-center bg-white shadow-sm border border-gray-200 rounded-xl p-4 max-w-xs"
        >
          {/* Blue circular icon */}
          <a href={meeting.meetLink} target="_blank" rel="noopener noreferrer">
            <div className="flex items-center justify-center w-20 h-24 mr-2 bg-blue-500 hover:bg-blue-600 text-white border">
              <VideoIcon className="w-8 h-8" />
            </div>
          </a>

          {/* Info section */}
          <div className="flex-1 ml-2">
            <p className="text-sm font-semibold text-gray-800">
              {meeting.user.fullName}
            </p>
            <p className="text-sm text-gray-600">
              {new Date(meeting.startDate).toDateString()}
            </p>
            <p className="text-sm text-gray-600">
              {new Date(meeting.startDate).toLocaleTimeString()} –{" "}
              {new Date(meeting.endDate).toLocaleTimeString()}
            </p>
            {/* <Button
              asChild
              size="sm"
              className="mt-2 bg-blue-600 hover:bg-blue-500"
            >
              <a href={meeting.meetLink} target="_blank" rel="noopener noreferrer">
                Join Meeting
              </a>
            </Button> */}
          </div>
        </div>
      ))}
    </div>
  );
};

export default UpcomingConsultantMeetings;
````

## File: Frontend/src/components/Filter.tsx
````typescript
import React, { useState } from "react";

interface FilterConfig {
  name: string;
  type: "text" | "number" | "select";
  placeholder: string;
  options?: string[]; // Only for select dropdowns
}

interface ReusableFilterProps {
  filtersConfig: FilterConfig[];
  onFilterChange: (filters: { [key: string]: string }) => void;
}

const Filter: React.FC<ReusableFilterProps> = ({ filtersConfig, onFilterChange }) => {
  const [filters, setFilters] = useState<{ [key: string]: string }>({});

  const handleApplyFilters = () => {
    onFilterChange(filters);
  };

  const handleResetFilters = () => {
    const resetFilters = filtersConfig.reduce((acc, filter) => {
      acc[filter.name] = "";
      return acc;
    }, {} as { [key: string]: string });
    
    setFilters(resetFilters);
    onFilterChange(resetFilters);
  };

  const handleFilterChange = (e: React.ChangeEvent<HTMLInputElement | HTMLSelectElement>) => {
    const { name, value } = e.target;
    setFilters({ ...filters, [name]: value });
  };

  return (
    <div className="p-4 shadow-md rounded-lg mb-4"> {/*removed bg-white*/}
      <h3 className="text-lg font-semibold mb-3">Filter Listings</h3>
      
      {/* Filter inputs in a grid layout */}
      <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
        {filtersConfig.map((filter) => (
          <div key={filter.name}>
            {filter.type === "select" ? (
              <select
                name={filter.name}
                value={filters[filter.name] || ""}
                onChange={handleFilterChange}
                className="border p-2 rounded w-full"
              >
                <option value="">{filter.placeholder}</option>
                {filter.options?.map((option) => (
                  <option key={option} value={option}>
                    {option}
                  </option>
                ))}
              </select>
            ) : (
              <input
                type={filter.type}
                name={filter.name}
                placeholder={filter.placeholder}
                value={filters[filter.name] || ""}
                onChange={handleFilterChange}
                className="border p-2 rounded w-full"
              />
            )}
          </div>
        ))}
      </div>

      {/* Buttons in a new row with spacing */}
      <div className="flex flex-wrap gap-4 mt-4 justify-center sm:justify-start">
        <button
          onClick={handleApplyFilters}
          className="bg-blue-500 hover:bg-blue-600 text-white font-semibold py-2 px-4 rounded transition duration-300"
        >
          Apply Filters
        </button>
        <button
          onClick={handleResetFilters}
          className="bg-red-500 hover:bg-red-600 text-white font-semibold py-2 px-4 rounded transition duration-300"
        >
          ✖ Reset Filters
        </button>
      </div>
    </div>
  );
};

export default Filter;
````

## File: Frontend/src/components/Footer.tsx
````typescript
import React from "react";
import Logo from "@/components/Logo";
import { IoLogoLinkedin } from "react-icons/io5";
import { FaXTwitter } from "react-icons/fa6";
import { FaInstagram } from "react-icons/fa";
import Link from "next/link";

export default function Footer() {
  return (
    <footer className="container mx-auto text-center py-10">
      <div className="flex justify-evenly flex-wrap">
        <div className="flex flex-col">
          <Logo path="/" />
          <p className="text-sm mt-2">&copy; 2025 ImmiGrow.A.I</p>
          <p className="text-sm">Edmonton, Alberta, Canada</p>
        </div>
        <div>
          <div className="flex justify-center mt-4 space-x-4">
            <Link
              href="https://www.linkedin.com/showcase/ImmiGrow-a-i/"
              aria-label="Linkedin"
            >
              <IoLogoLinkedin size={30} />
            </Link>
            <Link href="#" aria-label="X">
              <FaXTwitter size={30} />
            </Link>
            <Link href="#" aria-label="Instagram">
              <FaInstagram size={30} />
            </Link>
          </div>
        </div>
      </div>
      <div className="mt-6 px-4 text-sm">
        <p className="font-semibold">Land Acknowledgment</p>
        <p className="mt-2 md:px-40">
          At ImmiGrow.ai, we acknowledge that we operate on the traditional
          territories of Indigenous Peoples across Canada. We honor the rich
          history, culture, and contributions of First Nations, Métis, and Inuit
          communities. We are committed to fostering respectful relationships
          with Indigenous Peoples and recognizing their enduring presence and
          rights within their ancestral lands. As we work to support newcomers
          in their journey to Canada, we strive to promote equity, inclusion,
          and understanding for all.
        </p>
      </div>
    </footer>
  );
}
````

## File: Frontend/src/components/Header.tsx
````typescript
"use client";
import { useState } from "react";
import { FiMenu, FiX } from "react-icons/fi";
import Link from "next/link";
import { Button } from "@/components/ui/button";
import { usePathname } from "next/navigation";
import Logo from "./Logo";
import ThemeSwitcher from "./ThemeSwitcher";

export default function Header() {
  const [isMenuOpen, setIsMenuOpen] = useState(false);
  const pathname = usePathname();
  const isProtectedPath =
    pathname?.startsWith("/dashboard") || pathname?.startsWith("/onboarding");

  return (
    <header className="border-b border-border px-4 md:px-8 py-4 sticky top-0 z-50 w-full bg-background/95 backdrop-blur supports-[backdrop-filter]:bg-background/60">
      <nav className="flex justify-between items-center">
        <Logo path={pathname} />
        {/* Mobile Menu Toggle Button */}
        <button
          className="md:hidden p-2"
          onClick={() => setIsMenuOpen(!isMenuOpen)}
        >
          {isMenuOpen ? <FiX size={24} /> : <FiMenu size={24} />}
        </button>

        {/* Desktop Navigation */}

        {pathname.endsWith("/") && (
          <div className="hidden md:flex items-center gap-12">
            <Link href="#about">About</Link>
            <Link href="#testimonials">Testimonials</Link>
            <Link href="#contact">Contact</Link>
          </div>
        )}

        {/* Right Actions */}
        <div className="hidden md:flex items-center gap-4">
          {/* <ThemeSwitcher /> */}
          <Button className="bg-blue-600 hover:bg-blue-500">
            <Link href={isProtectedPath ? "/login" : "/login"}>
              {isProtectedPath ? "Logout" : "Login"}
            </Link>
          </Button>
        </div>
      </nav>

      {/* Mobile Navigation Menu */}
      {isMenuOpen && (
        <div className="md:hidden flex flex-col items-center gap-4 px-4 py-4">
          {pathname.endsWith("/") && (
            <>
              <Link href="/" onClick={() => setIsMenuOpen(false)}>
                About
              </Link>
              <Link href="/" onClick={() => setIsMenuOpen(false)}>
                Services
              </Link>
              <Link href="/" onClick={() => setIsMenuOpen(false)}>
                Contact
              </Link>
            </>
          )}
          <div className="flex flex-col items-center gap-4 mt-4">
            <ThemeSwitcher />
            <Button className="bg-blue-600 hover:bg-blue-500">
              <Link href={isProtectedPath ? "/logout" : "/login"}>
                {isProtectedPath ? "Logout" : "Login"}
              </Link>
            </Button>
          </div>
        </div>
      )}
    </header>
  );
}
````

## File: Frontend/src/components/ListingCard.tsx
````typescript
"use client";

import { useRouter, usePathname } from "next/navigation";
import { Card, CardContent, CardHeader } from "@/components/ui/card";
import { Bed, Bath, Clock, MapPin, DollarSign, Calendar } from "lucide-react";
import { TbBrandSpeedtest } from "react-icons/tb";

export default function ListingCard({ listing }) {
  const {
    id,
    title,
    location,
    price,
    houseImages,
    carImages,
    bedrooms,
    bathrooms,
    createdAt,
    make, // Used to determine car listing
    model,
    mileage,
    year,
  } = listing;

  const router = useRouter();
  const pathname = usePathname();

  const isCarListing = Boolean(make); // Check if the listing is a car
  const isHouseListing = Boolean(houseImages && houseImages.length > 0);

  const getSlicedPathname = (pathname: string) => {
    const pathArray = pathname.split("/");

    if (pathArray[1] === "dashboard" && pathArray[2] === "user") {
      return isCarListing
        ? `/${pathArray[1]}/${pathArray[2]}/cars`
        : `/${pathArray[1]}/${pathArray[2]}/homes`;
    }

    if (
      pathArray[1] === "dashboard" &&
      (pathArray[2] === "realtor" || pathArray[2] === "car-dealer")
    ) {
      return `/${pathArray[1]}/${pathArray[2]}`;
    }

    return pathArray.slice(0, pathArray.length - 1).join("/");
  };

  const handleCardClick = () => {
    if (isHouseListing) {
      router.push(`${getSlicedPathname(pathname)}/house-listings/${id}`);
    }
    if (isCarListing) {
      router.push(`${getSlicedPathname(pathname)}/car-listings/${id}`);
    }
  };

  return (
    <Card
      className="sm:w-full h-full border rounded-lg p-2 shadow-sm cursor-pointer hover:shadow-md transition flex"
      onClick={handleCardClick}
    >
      {/* Image Section */}
      <div className="w-1/3">
        {isHouseListing && (
          <img
            src={houseImages[0].base64}
            alt="House"
            className="w-full h-full object-cover rounded-l-lg"
          />
        )}
        {isCarListing && carImages?.length > 0 && (
          <img
            src={carImages[0].base64}
            alt="Car"
            className="w-full h-full object-cover rounded-l-lg"
          />
        )}
      </div>

      {/* Content Section */}
      <div className="w-2/3 p-2 flex flex-col justify-between">
        <CardHeader className="p-0">
          <div className="flex items-center justify-between">
            {title && (
              <p className="text-xl font-bold truncate w-30">{title}</p>
            )}
            {make && model && (
              <p className="text-xl font-bold">
                {model} {make}
              </p>
            )}
          </div>

          {/* Price */}
          <p className="text-xl font-bold text-blue-600 flex items-center">
            <DollarSign className="h-5 w-5 text-blue-600 mr-1" />
            {price.toLocaleString()}
          </p>

          {/* Location (Visible Only for Houses) */}
          {isHouseListing && (
            <p className="text-sm font-medium text-gray-700 flex items-start  gap-2">
              <MapPin size={20} />
              <span className="truncate w-50">{location}</span>
            </p>
          )}
          {isCarListing && (
            <p className="text-sm font-medium text-gray-700 flex items-start  gap-2">
              <Calendar size={20} />
              {year}
            </p>
          )}
        </CardHeader>

        {/* Features (House: Bedrooms & Bathrooms | Car: Just an Icon) */}
        <CardContent className="p-0 flex items-center space-x-4 text-gray-600 text-sm mt-2">
          {isHouseListing && bedrooms !== undefined && (
            <span className="flex items-center">
              <Bed className="h-4 w-4 mr-1" />
              {bedrooms}
            </span>
          )}
          {isHouseListing && bathrooms !== undefined && (
            <span className="flex items-center">
              <Bath className="h-4 w-4 mr-1" />
              {bathrooms}
            </span>
          )}
          {isCarListing && (
            <span className="flex items-center">
              <TbBrandSpeedtest className="h-4 w-4 mr-1" /> {mileage}
            </span>
          )}
          <span className="flex items-center">
            <Clock className="h-4 w-4 mr-1" />
            {createdAt ? new Date(createdAt).toDateString() : "Just now"}
          </span>
        </CardContent>
      </div>
    </Card>
  );
}
````

## File: Frontend/src/components/Listings.tsx
````typescript
'use client';

import { useState, useEffect } from 'react';
import ListingCard from './ListingCard';
import { Swiper, SwiperSlide } from 'swiper/react';
import { Navigation } from 'swiper/modules';
import 'swiper/css';
import 'swiper/css/navigation'; // Import the navigation styles

interface Listing {
  id: number;
  title: string;
  location?: string;
  price: number;
  imageUrl: string;
  description?: string | null;
  houseImages?: string[];
  carImages?: string[];
  make?: string;
  model?: string;
}

interface ListingsProps {
  listings: Listing[];
}


export default function Listings({ listings: initialListings }: ListingsProps) {
  const [listings, setListings] = useState<Listing[]>(initialListings);
  const [savedListings, setSavedListings] = useState<Set<number>>(new Set());

  // ✅ Sync state with updated listings from parent
  useEffect(() => {
    setListings(initialListings);
  }, [initialListings]);

  const handleSave = (listingId: number) => {
    setSavedListings((prev) => {
      const newSavedListings = new Set(prev);
      if (newSavedListings.has(listingId)) {
        newSavedListings.delete(listingId); // Unsave the listing
      } else {
        newSavedListings.add(listingId); // Save the listing
      }
      return newSavedListings;
    });
  };

  return (
    <Swiper
      modules={[Navigation]} // Ensure Navigation module is added
      spaceBetween={10}
      slidesPerView={3}
      navigation
      breakpoints={{
        1200: { slidesPerView: 3},
        1024: { slidesPerView: 3},
        768: { slidesPerView: 2 },
        480: { slidesPerView: 1 },
        0: { slidesPerView: 1 },
      }}
      style={{ width: '100%', overflow: 'hidden' }}
    >
      {listings.map((listing) => (
        <SwiperSlide key={listing.id}>
          <ListingCard
            listing={listing}
            isSaved={savedListings.has(listing.id)}
            onSave={handleSave}
          />
        </SwiperSlide>
      ))}
    </Swiper>
  );
}
````

## File: Frontend/src/components/Logo.tsx
````typescript
import Image from "next/image";
import Link from "next/link";
// import { usePathname } from "next/navigation";
import React from "react";
// import logo from "./public/logo.png";

const Logo = ({ path }: { path: string }) => {
  // const pathname = usePathname();
  const isProtectedPath =
    path?.startsWith("/dashboard") || path?.startsWith("/onboarding");
  return (
    <Link
      className="flex gap-1 justify-center items-center"
      href={isProtectedPath ? path : "/"}
    >
      <Image src={"/logo.png"} width={40} height={40} alt="ImmiGrow" />
      <p className="text-3xl font-bold tracking-tighter">ImmiGrow</p>
    </Link>
  );
};

export default Logo;
````

## File: Frontend/src/components/onboarding/DocumentUpload.tsx
````typescript
import React from "react";
import { Label } from "@/components/ui/label";
import { Input } from "@/components/ui/input";

interface DocumentUploadProps<T> {
  formData: T;
  setFormData: React.Dispatch<React.SetStateAction<T>>;
  errors: { [key: string]: string };
}

const DocumentUpload = <T extends Record<string, any>>({
  formData,
  setFormData,
  errors
}: DocumentUploadProps<T>) => {
  const handleFileChange = (
    e: React.ChangeEvent<HTMLInputElement>,
    field: keyof T
  ) => {
    if (e.target.files) {
      setFormData({ ...formData, [field]: e.target.files[0] });
    }
  };

  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Document Upload</h2>
      <div className="flex justify-between items-center">
        <Label>Government ID:</Label>
        <Input
          className="w-1/2 mb-4"
          type="file"
          onChange={(e) => handleFileChange(e, "governmentId")}
        />
      </div>
      {errors.governmentId && <p className="text-red-500 text-sm mb-4">{errors.governmentId}</p>}
      <div className="flex justify-between items-center">
        <Label>Business Verification:</Label>
        <Input
          className="w-1/2 mb-4"
          type="file"
          onChange={(e) => handleFileChange(e, "businessVerification")}
        />
      </div>
      {errors.businessVerification && <p className="text-red-500 text-sm mb-4">{errors.businessVerification}</p>}
      <div className="flex justify-between items-center">
        <Label>License Document:</Label>
        <Input
          className="w-1/2 mb-4"
          type="file"
          onChange={(e) => handleFileChange(e, "licenseDocument")}
        />
      </div>
      {errors.licenseDocument && <p className="text-red-500 text-sm mb-4">{errors.licenseDocument}</p>}
    </div>
  );
};

export default DocumentUpload;
````

## File: Frontend/src/components/onboarding/PersonalInformation.tsx
````typescript
"use client";

import React, { useState } from "react";
import { Input } from "@/components/ui/input";
import { Label } from "@/components/ui/label";
import {
  Popover,
  PopoverContent,
  PopoverTrigger,
} from "@/components/ui/popover";
import { CalendarIcon } from "lucide-react";
import { cn } from "@/lib/utils";
import { Button } from "@/components/ui/button";
import { Calendar } from "@/components/ui/calendar";
import { format } from "date-fns";

interface PersonalInformationProps<T> {
  formData: T;
  setFormData: React.Dispatch<React.SetStateAction<T>>;
  errors: { [key: string]: string };
}

const PersonalInformation = <T extends Record<string, any>>({
  formData,
  setFormData,
  errors,
}: PersonalInformationProps<T>) => {
  const [isOpen, setIsOpen] = useState(false);
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Personal Information</h2>
      <div className="flex justify-between items-center">
        <Label>Full Name:</Label>
        <Input
          className="w-2/3 mb-4"
          type="text"
          value={formData.fullName || ""}
          onChange={(e) =>
            setFormData({ ...formData, fullName: e.target.value })
          }
        />
      </div>
      {errors.fullName && <p className="text-red-500 text-sm mb-4">{errors.fullName}</p>}
      <div className="flex justify-between items-center">
        <Label>Phone Number:</Label>
        <Input
          className="w-2/3 mb-4"
          type="tel"
          value={formData.phoneNumber || ""}
          onChange={(e) =>
            setFormData({ ...formData, phoneNumber: e.target.value })
          }
        />
      </div>
      {errors.phoneNumber && <p className="text-red-500 text-sm mb-4">{errors.phoneNumber}</p>}
      {errors.phoneLength && <p className="text-red-500 text-sm mb-4">{errors.phoneLength}</p>}
      <div className="flex justify-between items-center">
        <Label>Date of Birth:</Label>
        <Popover open={isOpen} onOpenChange={setIsOpen}>
          <PopoverTrigger asChild>
            <Button
              variant={"outline"}
              className={cn(
                "w-2/3 mb-4",
                !formData.dateOfBirth && "text-muted-foreground"
              )}
            >
              {formData.dateOfBirth ? (
                format(formData.dateOfBirth, "PPP")
              ) : (
                <span>Date of Birth</span>
              )}
              <CalendarIcon className="ml-auto h-4 w-4 opacity-50" />
            </Button>
          </PopoverTrigger>
          <PopoverContent className="w-auto p-0" align="start">
            <Calendar
              mode="single"
              captionLayout="dropdown"
              selected={
                formData.dateOfBirth
                  ? new Date(formData.dateOfBirth)
                  : undefined
              }
              onSelect={(date) =>
                setFormData({
                  ...formData,
                  dateOfBirth: date ? date.toISOString().split("T")[0] : "",
                })
              }
              onDayClick={() => setIsOpen(false)}
              fromYear={1960}
              toYear={new Date().getFullYear()}
            />
          </PopoverContent>
        </Popover>
      </div>
      {errors.dateOfBirth && <p className="text-red-500 text-sm mb-4">{errors.dateOfBirth}</p>}
    </div>
  );
};

export default PersonalInformation;
````

## File: Frontend/src/components/onboarding/TermsAndConditions.tsx
````typescript
import React from "react";
import { Checkbox } from "@/components/ui/checkbox";
import { Label } from "@/components/ui/label";

interface TermsAndConditionsProps<T> {
  formData: T;
  setFormData: React.Dispatch<React.SetStateAction<T>>;
  errors: { [key: string]: string };
}

const TermsAndConditions = <T extends Record<string, any>>({
  formData,
  setFormData,
  errors,
}: TermsAndConditionsProps<T>) => {
  return (
    <div className="text-left">
      <h2 className="text-xl font-semibold mb-4">Terms and Conditions</h2>
      <div className="space-y-4">
        <div className="flex items-center space-x-2">
          <Checkbox
            checked={formData.backgroundCheckApproved || false} // Ensure it's a boolean
            onCheckedChange={(checked) => {
              setFormData({
                ...formData,
                backgroundCheckApproved: !!checked, // Convert to boolean
              });
            }}
          />
          <Label>I approve the background check.</Label>
        </div>
        {errors.backgroundCheckApproved && (
          <p className="text-red-500 text-sm mb-4">
            {errors.backgroundCheckApproved}
          </p>
        )}
        <div className="flex items-center space-x-2">
          <Checkbox
            checked={formData.termsAccepted || false} // Ensure it's a boolean
            onCheckedChange={(checked) =>
              setFormData({
                ...formData,
                termsAccepted: !!checked, // Convert to boolean
              })
            }
          />
          <Label>I agree to the terms and conditions.</Label>
        </div>
        {errors.termsAccepted && (
          <p className="text-red-500 text-sm mb-4">
            {errors.termsAccepted}
          </p>
        )}
      </div>
    </div>
  );
};

export default TermsAndConditions;
````

## File: Frontend/src/components/providers/theme-provider.tsx
````typescript
"use client";

import * as React from "react";
import { ThemeProvider as NextThemesProvider } from "next-themes";

export function ThemeProvider({
  children,
  ...props
}: React.ComponentProps<typeof NextThemesProvider>) {
  return <NextThemesProvider {...props}>{children}</NextThemesProvider>;
}
````

## File: Frontend/src/components/QuickLinks.tsx
````typescript
import { Card } from "@/components/ui/card";
import { buttonVariants } from "@/components/ui/button";

export default function QuickLinks({ links }: { links: { label: string; href: string }[] }) {
  return (
    <Card>
      <div className="p-4">
        <h2 className="text-lg font-semibold mb-2">Quick Links</h2>
        <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-5 2xl:grid-cols-6 gap-2">
          {links.map((link, index) => (
            <a
              key={index}
              href={link.href}
              className={buttonVariants({
                variant: "outline",
                size: "lg", 
                className: "w-full",
              })}
            >
              {link.label}
            </a>
          ))}
        </div>
      </div>
    </Card>
  );
}
````

## File: Frontend/src/components/Sidecard.tsx
````typescript
import { Card } from "@/components/ui/card";
import { buttonVariants } from "@/components/ui/button";
import Link from "next/link";

interface SideCardProps {
  services: string[];
  title: string;
  urls: string[];
}

export default function SideCard({ services, title, urls }: SideCardProps) {
  return (
    <Card className="md:h-full">
      <div className="p-4">
        <h2 className="text-2xl font-bold mb-4 text-center">{title}</h2>
        <ul>
          {services.map((service, index) => (
            <li key={index} className="mb-2">
              <Link
                href={urls[index]}
                className={buttonVariants({
                  variant: "ghost",
                  size: "lg",
                  className: "w-full justify-start",
                })}
              >
                {service}
              </Link>
            </li>
          ))}
        </ul>
      </div>
    </Card>
  );
}
````

## File: Frontend/src/components/ThemeSwitcher.tsx
````typescript
"use client";

import { useTheme } from "next-themes";
import React, { useEffect } from "react";
import { Tabs, TabsList, TabsTrigger } from "@/components/ui/tabs";
import { FaSun, FaMoon, FaLaptop } from "react-icons/fa";

function ThemeSwitcher() {
  const { theme, setTheme } = useTheme();
  const [mounted, setMounted] = React.useState(false);

  useEffect(() => {
    setMounted(true);
  }, []);

  if (!mounted) return null;

  return (
    <Tabs defaultValue={theme}>
      <TabsList className="border">
        <TabsTrigger value="light" onClick={() => setTheme("light")}>
          <FaSun size={16} />
        </TabsTrigger>
        <TabsTrigger value="dark" onClick={() => setTheme("dark")}>
          <FaMoon size={16} />
        </TabsTrigger>
        <TabsTrigger value="system" onClick={() => setTheme("system")}>
          <FaLaptop size={16} />
        </TabsTrigger>
      </TabsList>
    </Tabs>
  );
}

export default ThemeSwitcher;
````

## File: Frontend/src/components/ui/alert.tsx
````typescript
import * as React from "react"
import { cva, type VariantProps } from "class-variance-authority"

import { cn } from "@/lib/utils"

const alertVariants = cva(
  "relative w-full rounded-lg border px-4 py-3 text-sm [&>svg+div]:translate-y-[-3px] [&>svg]:absolute [&>svg]:left-4 [&>svg]:top-4 [&>svg]:text-foreground [&>svg~*]:pl-7",
  {
    variants: {
      variant: {
        default: "bg-background text-foreground",
        destructive:
          "border-destructive/50 text-destructive dark:border-destructive [&>svg]:text-destructive",
      },
    },
    defaultVariants: {
      variant: "default",
    },
  }
)

const Alert = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement> & VariantProps<typeof alertVariants>
>(({ className, variant, ...props }, ref) => (
  <div
    ref={ref}
    role="alert"
    className={cn(alertVariants({ variant }), className)}
    {...props}
  />
))
Alert.displayName = "Alert"

const AlertTitle = React.forwardRef<
  HTMLParagraphElement,
  React.HTMLAttributes<HTMLHeadingElement>
>(({ className, ...props }, ref) => (
  <h5
    ref={ref}
    className={cn("mb-1 font-medium leading-none tracking-tight", className)}
    {...props}
  />
))
AlertTitle.displayName = "AlertTitle"

const AlertDescription = React.forwardRef<
  HTMLParagraphElement,
  React.HTMLAttributes<HTMLParagraphElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("text-sm [&_p]:leading-relaxed", className)}
    {...props}
  />
))
AlertDescription.displayName = "AlertDescription"

export { Alert, AlertTitle, AlertDescription }
````

## File: Frontend/src/components/ui/button.tsx
````typescript
import * as React from "react"
import { Slot } from "@radix-ui/react-slot"
import { cva, type VariantProps } from "class-variance-authority"

import { cn } from "@/lib/utils"

const buttonVariants = cva(
  "inline-flex items-center justify-center gap-2 whitespace-nowrap rounded-md text-sm font-medium transition-colors focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:pointer-events-none disabled:opacity-50 [&_svg]:pointer-events-none [&_svg]:size-4 [&_svg]:shrink-0",
  {
    variants: {
      variant: {
        default:
          "bg-primary text-primary-foreground shadow hover:bg-primary/90",
        destructive:
          "bg-destructive text-destructive-foreground shadow-sm hover:bg-destructive/90",
        outline:
          "border border-input bg-background shadow-sm hover:bg-accent hover:text-accent-foreground",
        secondary:
          "bg-secondary text-secondary-foreground shadow-sm hover:bg-secondary/80",
        ghost: "hover:bg-accent hover:text-accent-foreground",
        link: "text-primary underline-offset-4 hover:underline",
      },
      size: {
        default: "h-9 px-4 py-2",
        sm: "h-8 rounded-md px-3 text-xs",
        lg: "h-10 rounded-md px-8",
        icon: "h-9 w-9",
      },
    },
    defaultVariants: {
      variant: "default",
      size: "default",
    },
  }
)

export interface ButtonProps
  extends React.ButtonHTMLAttributes<HTMLButtonElement>,
    VariantProps<typeof buttonVariants> {
  asChild?: boolean
}

const Button = React.forwardRef<HTMLButtonElement, ButtonProps>(
  ({ className, variant, size, asChild = false, ...props }, ref) => {
    const Comp = asChild ? Slot : "button"
    return (
      <Comp
        className={cn(buttonVariants({ variant, size, className }))}
        ref={ref}
        {...props}
      />
    )
  }
)
Button.displayName = "Button"

export { Button, buttonVariants }
````

## File: Frontend/src/components/ui/calendar.tsx
````typescript
"use client";

import * as React from "react";
import { ChevronLeft, ChevronRight } from "lucide-react";
import { DayPicker, DropdownProps } from "react-day-picker";

import { cn } from "@/lib/utils";
import { buttonVariants } from "@/components/ui/button";
import {
  Select,
  SelectContent,
  SelectItem,
  SelectTrigger,
  SelectValue,
} from "./select";
import { ScrollArea } from "@/components/ui/scroll-area";

export type CalendarProps = React.ComponentProps<typeof DayPicker>;

function Calendar({
  className,
  classNames,
  showOutsideDays = true,
  ...props
}: CalendarProps) {
  return (
    <DayPicker
      showOutsideDays={showOutsideDays}
      className={cn("p-3", className)}
      classNames={{
        month: "space-y-4",
        months: "flex flex-col sm:flex-row space-y-4 sm:space-y-0 relative",
        month_caption: "flex justify-center pt-1 relative items-center",
        month_grid: "w-full border-collapse space-y-1",

        // TEST
        dropdowns: "flex justify-center gap-1",
        nav: "flex items-center justify-between absolute inset-x-0 top-2",
        button_previous: cn(
          buttonVariants({ variant: "outline" }),
          "h-7 w-7 bg-transparent p-0 opacity-50 hover:opacity-100 z-10"
        ),
        button_next: cn(
          buttonVariants({ variant: "outline" }),
          "h-7 w-7 bg-transparent p-0 opacity-50 hover:opacity-100 z-10"
        ),
        // TEST

        weeks: "w-full border-collapse space-y-",
        weekdays: "flex",
        weekday:
          "text-muted-foreground rounded-md w-9 font-normal text-[0.8rem]",
        week: "flex w-full mt-2",
        day_button:
          "h-9 w-9 text-center text-sm p-0 relative [&:has([aria-selected].day-range-end)]:rounded-r-md [&:has([aria-selected].day-outside)]:bg-accent/50 [&:has([aria-selected])]:bg-accent first:[&:has([aria-selected])]:rounded-l-md last:[&:has([aria-selected])]:rounded-r-md focus-within:relative focus-within:z-20",
        day: cn(
          buttonVariants({ variant: "ghost" }),
          "h-9 w-9 p-0 font-normal aria-selected:opacity-100"
        ),
        range_end: "day-range-end",
        selected:
          "bg-primary text-primary-foreground hover:bg-primary hover:text-primary-foreground focus:bg-primary focus:text-primary-foreground",
        outside:
          "day-outside text-muted-foreground opacity-50 aria-selected:bg-accent/50 aria-selected:text-muted-foreground aria-selected:opacity-30",
        disabled: "text-muted-foreground opacity-50",
        range_middle:
          "aria-selected:bg-accent aria-selected:text-accent-foreground",
        hidden: "invisible",
        ...classNames,
      }}
      components={{
        Dropdown: ({ value, onChange, options }: DropdownProps) => {
          const selected = options?.find((child) => child.value === value);
          const handleChange = (value: string) => {
            const changeEvent = {
              target: { value },
            } as React.ChangeEvent<HTMLSelectElement>;
            onChange?.(changeEvent);
          };
          return (
            <Select
              value={value?.toString()}
              onValueChange={(value) => {
                handleChange(value);
              }}
            >
              <SelectTrigger className="pr-1.5 focus:ring-0">
                <SelectValue>{selected?.label}</SelectValue>
              </SelectTrigger>
              <SelectContent position="popper">
                <ScrollArea className="h-80">
                  {options?.map((option, id: number) => (
                    <SelectItem
                      key={`${option.value}-${id}`}
                      value={option.value?.toString() ?? ""}
                    >
                      {option.label}
                    </SelectItem>
                  ))}
                </ScrollArea>
              </SelectContent>
            </Select>
          );
        },
        Chevron: ({ ...props }) =>
          props.orientation === "left" ? (
            <ChevronLeft {...props} className="h-4 w-4" />
          ) : (
            <ChevronRight {...props} className="h-4 w-4" />
          ),
      }}
      {...props}
    />
  );
}
Calendar.displayName = "Calendar";

export { Calendar };
````

## File: Frontend/src/components/ui/card.tsx
````typescript
import * as React from "react"

import { cn } from "@/lib/utils"

const Card = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn(
      "rounded-xl border bg-card text-card-foreground shadow",
      className
    )}
    {...props}
  />
))
Card.displayName = "Card"

const CardHeader = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("flex flex-col space-y-1.5 p-6", className)}
    {...props}
  />
))
CardHeader.displayName = "CardHeader"

const CardTitle = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("font-semibold leading-none tracking-tight", className)}
    {...props}
  />
))
CardTitle.displayName = "CardTitle"

const CardDescription = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props}
  />
))
CardDescription.displayName = "CardDescription"

const CardContent = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div ref={ref} className={cn("p-6 pt-0", className)} {...props} />
))
CardContent.displayName = "CardContent"

const CardFooter = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => (
  <div
    ref={ref}
    className={cn("flex items-center p-6 pt-0", className)}
    {...props}
  />
))
CardFooter.displayName = "CardFooter"

export { Card, CardHeader, CardFooter, CardTitle, CardDescription, CardContent }
````

## File: Frontend/src/components/ui/chart.tsx
````typescript
"use client"

import * as React from "react"
import * as RechartsPrimitive from "recharts"

import { cn } from "@/lib/utils"

// Format: { THEME_NAME: CSS_SELECTOR }
const THEMES = { light: "", dark: ".dark" } as const

export type ChartConfig = {
  [k in string]: {
    label?: React.ReactNode
    icon?: React.ComponentType
  } & (
    | { color?: string; theme?: never }
    | { color?: never; theme: Record<keyof typeof THEMES, string> }
  )
}

type ChartContextProps = {
  config: ChartConfig
}

const ChartContext = React.createContext<ChartContextProps | null>(null)

function useChart() {
  const context = React.useContext(ChartContext)

  if (!context) {
    throw new Error("useChart must be used within a <ChartContainer />")
  }

  return context
}

const ChartContainer = React.forwardRef<
  HTMLDivElement,
  React.ComponentProps<"div"> & {
    config: ChartConfig
    children: React.ComponentProps<
      typeof RechartsPrimitive.ResponsiveContainer
    >["children"]
  }
>(({ id, className, children, config, ...props }, ref) => {
  const uniqueId = React.useId()
  const chartId = `chart-${id || uniqueId.replace(/:/g, "")}`

  return (
    <ChartContext.Provider value={{ config }}>
      <div
        data-chart={chartId}
        ref={ref}
        className={cn(
          "flex aspect-video justify-center text-xs [&_.recharts-cartesian-axis-tick_text]:fill-muted-foreground [&_.recharts-cartesian-grid_line[stroke='#ccc']]:stroke-border/50 [&_.recharts-curve.recharts-tooltip-cursor]:stroke-border [&_.recharts-dot[stroke='#fff']]:stroke-transparent [&_.recharts-layer]:outline-none [&_.recharts-polar-grid_[stroke='#ccc']]:stroke-border [&_.recharts-radial-bar-background-sector]:fill-muted [&_.recharts-rectangle.recharts-tooltip-cursor]:fill-muted [&_.recharts-reference-line_[stroke='#ccc']]:stroke-border [&_.recharts-sector[stroke='#fff']]:stroke-transparent [&_.recharts-sector]:outline-none [&_.recharts-surface]:outline-none",
          className
        )}
        {...props}
      >
        <ChartStyle id={chartId} config={config} />
        <RechartsPrimitive.ResponsiveContainer>
          {children}
        </RechartsPrimitive.ResponsiveContainer>
      </div>
    </ChartContext.Provider>
  )
})
ChartContainer.displayName = "Chart"

const ChartStyle = ({ id, config }: { id: string; config: ChartConfig }) => {
  const colorConfig = Object.entries(config).filter(
    ([, config]) => config.theme || config.color
  )

  if (!colorConfig.length) {
    return null
  }

  return (
    <style
      dangerouslySetInnerHTML={{
        __html: Object.entries(THEMES)
          .map(
            ([theme, prefix]) => `
${prefix} [data-chart=${id}] {
${colorConfig
  .map(([key, itemConfig]) => {
    const color =
      itemConfig.theme?.[theme as keyof typeof itemConfig.theme] ||
      itemConfig.color
    return color ? `  --color-${key}: ${color};` : null
  })
  .join("\n")}
}
`
          )
          .join("\n"),
      }}
    />
  )
}

const ChartTooltip = RechartsPrimitive.Tooltip

const ChartTooltipContent = React.forwardRef<
  HTMLDivElement,
  React.ComponentProps<typeof RechartsPrimitive.Tooltip> &
    React.ComponentProps<"div"> & {
      hideLabel?: boolean
      hideIndicator?: boolean
      indicator?: "line" | "dot" | "dashed"
      nameKey?: string
      labelKey?: string
    }
>(
  (
    {
      active,
      payload,
      className,
      indicator = "dot",
      hideLabel = false,
      hideIndicator = false,
      label,
      labelFormatter,
      labelClassName,
      formatter,
      color,
      nameKey,
      labelKey,
    },
    ref
  ) => {
    const { config } = useChart()

    const tooltipLabel = React.useMemo(() => {
      if (hideLabel || !payload?.length) {
        return null
      }

      const [item] = payload
      const key = `${labelKey || item?.dataKey || item?.name || "value"}`
      const itemConfig = getPayloadConfigFromPayload(config, item, key)
      const value =
        !labelKey && typeof label === "string"
          ? config[label as keyof typeof config]?.label || label
          : itemConfig?.label

      if (labelFormatter) {
        return (
          <div className={cn("font-medium", labelClassName)}>
            {labelFormatter(value, payload)}
          </div>
        )
      }

      if (!value) {
        return null
      }

      return <div className={cn("font-medium", labelClassName)}>{value}</div>
    }, [
      label,
      labelFormatter,
      payload,
      hideLabel,
      labelClassName,
      config,
      labelKey,
    ])

    if (!active || !payload?.length) {
      return null
    }

    const nestLabel = payload.length === 1 && indicator !== "dot"

    return (
      <div
        ref={ref}
        className={cn(
          "grid min-w-[8rem] items-start gap-1.5 rounded-lg border border-border/50 bg-background px-2.5 py-1.5 text-xs shadow-xl",
          className
        )}
      >
        {!nestLabel ? tooltipLabel : null}
        <div className="grid gap-1.5">
          {payload.map((item, index) => {
            const key = `${nameKey || item.name || item.dataKey || "value"}`
            const itemConfig = getPayloadConfigFromPayload(config, item, key)
            const indicatorColor = color || item.payload.fill || item.color

            return (
              <div
                key={item.dataKey}
                className={cn(
                  "flex w-full flex-wrap items-stretch gap-2 [&>svg]:h-2.5 [&>svg]:w-2.5 [&>svg]:text-muted-foreground",
                  indicator === "dot" && "items-center"
                )}
              >
                {formatter && item?.value !== undefined && item.name ? (
                  formatter(item.value, item.name, item, index, item.payload)
                ) : (
                  <>
                    {itemConfig?.icon ? (
                      <itemConfig.icon />
                    ) : (
                      !hideIndicator && (
                        <div
                          className={cn(
                            "shrink-0 rounded-[2px] border-[--color-border] bg-[--color-bg]",
                            {
                              "h-2.5 w-2.5": indicator === "dot",
                              "w-1": indicator === "line",
                              "w-0 border-[1.5px] border-dashed bg-transparent":
                                indicator === "dashed",
                              "my-0.5": nestLabel && indicator === "dashed",
                            }
                          )}
                          style={
                            {
                              "--color-bg": indicatorColor,
                              "--color-border": indicatorColor,
                            } as React.CSSProperties
                          }
                        />
                      )
                    )}
                    <div
                      className={cn(
                        "flex flex-1 justify-between leading-none",
                        nestLabel ? "items-end" : "items-center"
                      )}
                    >
                      <div className="grid gap-1.5">
                        {nestLabel ? tooltipLabel : null}
                        <span className="text-muted-foreground">
                          {itemConfig?.label || item.name}
                        </span>
                      </div>
                      {item.value && (
                        <span className="font-mono font-medium tabular-nums text-foreground">
                          {item.value.toLocaleString()}
                        </span>
                      )}
                    </div>
                  </>
                )}
              </div>
            )
          })}
        </div>
      </div>
    )
  }
)
ChartTooltipContent.displayName = "ChartTooltip"

const ChartLegend = RechartsPrimitive.Legend

const ChartLegendContent = React.forwardRef<
  HTMLDivElement,
  React.ComponentProps<"div"> &
    Pick<RechartsPrimitive.LegendProps, "payload" | "verticalAlign"> & {
      hideIcon?: boolean
      nameKey?: string
    }
>(
  (
    { className, hideIcon = false, payload, verticalAlign = "bottom", nameKey },
    ref
  ) => {
    const { config } = useChart()

    if (!payload?.length) {
      return null
    }

    return (
      <div
        ref={ref}
        className={cn(
          "flex items-center justify-center gap-4",
          verticalAlign === "top" ? "pb-3" : "pt-3",
          className
        )}
      >
        {payload.map((item) => {
          const key = `${nameKey || item.dataKey || "value"}`
          const itemConfig = getPayloadConfigFromPayload(config, item, key)

          return (
            <div
              key={item.value}
              className={cn(
                "flex items-center gap-1.5 [&>svg]:h-3 [&>svg]:w-3 [&>svg]:text-muted-foreground"
              )}
            >
              {itemConfig?.icon && !hideIcon ? (
                <itemConfig.icon />
              ) : (
                <div
                  className="h-2 w-2 shrink-0 rounded-[2px]"
                  style={{
                    backgroundColor: item.color,
                  }}
                />
              )}
              {itemConfig?.label}
            </div>
          )
        })}
      </div>
    )
  }
)
ChartLegendContent.displayName = "ChartLegend"

// Helper to extract item config from a payload.
function getPayloadConfigFromPayload(
  config: ChartConfig,
  payload: unknown,
  key: string
) {
  if (typeof payload !== "object" || payload === null) {
    return undefined
  }

  const payloadPayload =
    "payload" in payload &&
    typeof payload.payload === "object" &&
    payload.payload !== null
      ? payload.payload
      : undefined

  let configLabelKey: string = key

  if (
    key in payload &&
    typeof payload[key as keyof typeof payload] === "string"
  ) {
    configLabelKey = payload[key as keyof typeof payload] as string
  } else if (
    payloadPayload &&
    key in payloadPayload &&
    typeof payloadPayload[key as keyof typeof payloadPayload] === "string"
  ) {
    configLabelKey = payloadPayload[
      key as keyof typeof payloadPayload
    ] as string
  }

  return configLabelKey in config
    ? config[configLabelKey]
    : config[key as keyof typeof config]
}

export {
  ChartContainer,
  ChartTooltip,
  ChartTooltipContent,
  ChartLegend,
  ChartLegendContent,
  ChartStyle,
}
````

## File: Frontend/src/components/ui/checkbox.tsx
````typescript
"use client"

import * as React from "react"
import * as CheckboxPrimitive from "@radix-ui/react-checkbox"
import { Check } from "lucide-react"

import { cn } from "@/lib/utils"

const Checkbox = React.forwardRef<
  React.ElementRef<typeof CheckboxPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof CheckboxPrimitive.Root>
>(({ className, ...props }, ref) => (
  <CheckboxPrimitive.Root
    ref={ref}
    className={cn(
      "peer h-4 w-4 shrink-0 rounded-sm border border-primary shadow focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 data-[state=checked]:bg-primary data-[state=checked]:text-primary-foreground",
      className
    )}
    {...props}
  >
    <CheckboxPrimitive.Indicator
      className={cn("flex items-center justify-center text-current")}
    >
      <Check className="h-4 w-4" />
    </CheckboxPrimitive.Indicator>
  </CheckboxPrimitive.Root>
))
Checkbox.displayName = CheckboxPrimitive.Root.displayName

export { Checkbox }
````

## File: Frontend/src/components/ui/dialog.tsx
````typescript
"use client"

import * as React from "react"
import * as DialogPrimitive from "@radix-ui/react-dialog"
import { X } from "lucide-react"

import { cn } from "@/lib/utils"

const Dialog = DialogPrimitive.Root

const DialogTrigger = DialogPrimitive.Trigger

const DialogPortal = DialogPrimitive.Portal

const DialogClose = DialogPrimitive.Close

const DialogOverlay = React.forwardRef<
  React.ElementRef<typeof DialogPrimitive.Overlay>,
  React.ComponentPropsWithoutRef<typeof DialogPrimitive.Overlay>
>(({ className, ...props }, ref) => (
  <DialogPrimitive.Overlay
    ref={ref}
    className={cn(
      "fixed inset-0 z-50 bg-black/80  data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0",
      className
    )}
    {...props}
  />
))
DialogOverlay.displayName = DialogPrimitive.Overlay.displayName

const DialogContent = React.forwardRef<
  React.ElementRef<typeof DialogPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof DialogPrimitive.Content>
>(({ className, children, ...props }, ref) => (
  <DialogPortal>
    <DialogOverlay />
    <DialogPrimitive.Content
      ref={ref}
      className={cn(
        "fixed left-[50%] top-[50%] z-50 grid w-full max-w-lg translate-x-[-50%] translate-y-[-50%] gap-4 border bg-background p-6 shadow-lg duration-200 data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[state=closed]:slide-out-to-left-1/2 data-[state=closed]:slide-out-to-top-[48%] data-[state=open]:slide-in-from-left-1/2 data-[state=open]:slide-in-from-top-[48%] sm:rounded-lg",
        className
      )}
      {...props}
    >
      {children}
      <DialogPrimitive.Close className="absolute right-4 top-4 rounded-sm opacity-70 ring-offset-background transition-opacity hover:opacity-100 focus:outline-none focus:ring-2 focus:ring-ring focus:ring-offset-2 disabled:pointer-events-none data-[state=open]:bg-accent data-[state=open]:text-muted-foreground">
        <X className="h-4 w-4" />
        <span className="sr-only">Close</span>
      </DialogPrimitive.Close>
    </DialogPrimitive.Content>
  </DialogPortal>
))
DialogContent.displayName = DialogPrimitive.Content.displayName

const DialogHeader = ({
  className,
  ...props
}: React.HTMLAttributes<HTMLDivElement>) => (
  <div
    className={cn(
      "flex flex-col space-y-1.5 text-center sm:text-left",
      className
    )}
    {...props}
  />
)
DialogHeader.displayName = "DialogHeader"

const DialogFooter = ({
  className,
  ...props
}: React.HTMLAttributes<HTMLDivElement>) => (
  <div
    className={cn(
      "flex flex-col-reverse sm:flex-row sm:justify-end sm:space-x-2",
      className
    )}
    {...props}
  />
)
DialogFooter.displayName = "DialogFooter"

const DialogTitle = React.forwardRef<
  React.ElementRef<typeof DialogPrimitive.Title>,
  React.ComponentPropsWithoutRef<typeof DialogPrimitive.Title>
>(({ className, ...props }, ref) => (
  <DialogPrimitive.Title
    ref={ref}
    className={cn(
      "text-lg font-semibold leading-none tracking-tight",
      className
    )}
    {...props}
  />
))
DialogTitle.displayName = DialogPrimitive.Title.displayName

const DialogDescription = React.forwardRef<
  React.ElementRef<typeof DialogPrimitive.Description>,
  React.ComponentPropsWithoutRef<typeof DialogPrimitive.Description>
>(({ className, ...props }, ref) => (
  <DialogPrimitive.Description
    ref={ref}
    className={cn("text-sm text-muted-foreground", className)}
    {...props}
  />
))
DialogDescription.displayName = DialogPrimitive.Description.displayName

export {
  Dialog,
  DialogPortal,
  DialogOverlay,
  DialogTrigger,
  DialogClose,
  DialogContent,
  DialogHeader,
  DialogFooter,
  DialogTitle,
  DialogDescription,
}
````

## File: Frontend/src/components/ui/dropdown-menu.tsx
````typescript
"use client"

import * as React from "react"
import * as DropdownMenuPrimitive from "@radix-ui/react-dropdown-menu"
import { Check, ChevronRight, Circle } from "lucide-react"

import { cn } from "@/lib/utils"

const DropdownMenu = DropdownMenuPrimitive.Root

const DropdownMenuTrigger = DropdownMenuPrimitive.Trigger

const DropdownMenuGroup = DropdownMenuPrimitive.Group

const DropdownMenuPortal = DropdownMenuPrimitive.Portal

const DropdownMenuSub = DropdownMenuPrimitive.Sub

const DropdownMenuRadioGroup = DropdownMenuPrimitive.RadioGroup

const DropdownMenuSubTrigger = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.SubTrigger>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.SubTrigger> & {
    inset?: boolean
  }
>(({ className, inset, children, ...props }, ref) => (
  <DropdownMenuPrimitive.SubTrigger
    ref={ref}
    className={cn(
      "flex cursor-default select-none items-center gap-2 rounded-sm px-2 py-1.5 text-sm outline-none focus:bg-accent data-[state=open]:bg-accent [&_svg]:pointer-events-none [&_svg]:size-4 [&_svg]:shrink-0",
      inset && "pl-8",
      className
    )}
    {...props}
  >
    {children}
    <ChevronRight className="ml-auto" />
  </DropdownMenuPrimitive.SubTrigger>
))
DropdownMenuSubTrigger.displayName =
  DropdownMenuPrimitive.SubTrigger.displayName

const DropdownMenuSubContent = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.SubContent>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.SubContent>
>(({ className, ...props }, ref) => (
  <DropdownMenuPrimitive.SubContent
    ref={ref}
    className={cn(
      "z-50 min-w-[8rem] overflow-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-lg data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
      className
    )}
    {...props}
  />
))
DropdownMenuSubContent.displayName =
  DropdownMenuPrimitive.SubContent.displayName

const DropdownMenuContent = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.Content>
>(({ className, sideOffset = 4, ...props }, ref) => (
  <DropdownMenuPrimitive.Portal>
    <DropdownMenuPrimitive.Content
      ref={ref}
      sideOffset={sideOffset}
      className={cn(
        "z-50 max-h-[var(--radix-dropdown-menu-content-available-height)] min-w-[8rem] overflow-y-auto overflow-x-hidden rounded-md border bg-popover p-1 text-popover-foreground shadow-md",
        "data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props}
    />
  </DropdownMenuPrimitive.Portal>
))
DropdownMenuContent.displayName = DropdownMenuPrimitive.Content.displayName

const DropdownMenuItem = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.Item>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.Item> & {
    inset?: boolean
  }
>(({ className, inset, ...props }, ref) => (
  <DropdownMenuPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center gap-2 rounded-sm px-2 py-1.5 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50 [&>svg]:size-4 [&>svg]:shrink-0",
      inset && "pl-8",
      className
    )}
    {...props}
  />
))
DropdownMenuItem.displayName = DropdownMenuPrimitive.Item.displayName

const DropdownMenuCheckboxItem = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.CheckboxItem>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.CheckboxItem>
>(({ className, children, checked, ...props }, ref) => (
  <DropdownMenuPrimitive.CheckboxItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    checked={checked}
    {...props}
  >
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <DropdownMenuPrimitive.ItemIndicator>
        <Check className="h-4 w-4" />
      </DropdownMenuPrimitive.ItemIndicator>
    </span>
    {children}
  </DropdownMenuPrimitive.CheckboxItem>
))
DropdownMenuCheckboxItem.displayName =
  DropdownMenuPrimitive.CheckboxItem.displayName

const DropdownMenuRadioItem = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.RadioItem>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.RadioItem>
>(({ className, children, ...props }, ref) => (
  <DropdownMenuPrimitive.RadioItem
    ref={ref}
    className={cn(
      "relative flex cursor-default select-none items-center rounded-sm py-1.5 pl-8 pr-2 text-sm outline-none transition-colors focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    {...props}
  >
    <span className="absolute left-2 flex h-3.5 w-3.5 items-center justify-center">
      <DropdownMenuPrimitive.ItemIndicator>
        <Circle className="h-2 w-2 fill-current" />
      </DropdownMenuPrimitive.ItemIndicator>
    </span>
    {children}
  </DropdownMenuPrimitive.RadioItem>
))
DropdownMenuRadioItem.displayName = DropdownMenuPrimitive.RadioItem.displayName

const DropdownMenuLabel = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.Label>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.Label> & {
    inset?: boolean
  }
>(({ className, inset, ...props }, ref) => (
  <DropdownMenuPrimitive.Label
    ref={ref}
    className={cn(
      "px-2 py-1.5 text-sm font-semibold",
      inset && "pl-8",
      className
    )}
    {...props}
  />
))
DropdownMenuLabel.displayName = DropdownMenuPrimitive.Label.displayName

const DropdownMenuSeparator = React.forwardRef<
  React.ElementRef<typeof DropdownMenuPrimitive.Separator>,
  React.ComponentPropsWithoutRef<typeof DropdownMenuPrimitive.Separator>
>(({ className, ...props }, ref) => (
  <DropdownMenuPrimitive.Separator
    ref={ref}
    className={cn("-mx-1 my-1 h-px bg-muted", className)}
    {...props}
  />
))
DropdownMenuSeparator.displayName = DropdownMenuPrimitive.Separator.displayName

const DropdownMenuShortcut = ({
  className,
  ...props
}: React.HTMLAttributes<HTMLSpanElement>) => {
  return (
    <span
      className={cn("ml-auto text-xs tracking-widest opacity-60", className)}
      {...props}
    />
  )
}
DropdownMenuShortcut.displayName = "DropdownMenuShortcut"

export {
  DropdownMenu,
  DropdownMenuTrigger,
  DropdownMenuContent,
  DropdownMenuItem,
  DropdownMenuCheckboxItem,
  DropdownMenuRadioItem,
  DropdownMenuLabel,
  DropdownMenuSeparator,
  DropdownMenuShortcut,
  DropdownMenuGroup,
  DropdownMenuPortal,
  DropdownMenuSub,
  DropdownMenuSubContent,
  DropdownMenuSubTrigger,
  DropdownMenuRadioGroup,
}
````

## File: Frontend/src/components/ui/form.tsx
````typescript
"use client"

import * as React from "react"
import * as LabelPrimitive from "@radix-ui/react-label"
import { Slot } from "@radix-ui/react-slot"
import {
  Controller,
  ControllerProps,
  FieldPath,
  FieldValues,
  FormProvider,
  useFormContext,
} from "react-hook-form"

import { cn } from "@/lib/utils"
import { Label } from "@/components/ui/label"

const Form = FormProvider

type FormFieldContextValue<
  TFieldValues extends FieldValues = FieldValues,
  TName extends FieldPath<TFieldValues> = FieldPath<TFieldValues>
> = {
  name: TName
}

const FormFieldContext = React.createContext<FormFieldContextValue>(
  {} as FormFieldContextValue
)

const FormField = <
  TFieldValues extends FieldValues = FieldValues,
  TName extends FieldPath<TFieldValues> = FieldPath<TFieldValues>
>({
  ...props
}: ControllerProps<TFieldValues, TName>) => {
  return (
    <FormFieldContext.Provider value={{ name: props.name }}>
      <Controller {...props} />
    </FormFieldContext.Provider>
  )
}

const useFormField = () => {
  const fieldContext = React.useContext(FormFieldContext)
  const itemContext = React.useContext(FormItemContext)
  const { getFieldState, formState } = useFormContext()

  const fieldState = getFieldState(fieldContext.name, formState)

  if (!fieldContext) {
    throw new Error("useFormField should be used within <FormField>")
  }

  const { id } = itemContext

  return {
    id,
    name: fieldContext.name,
    formItemId: `${id}-form-item`,
    formDescriptionId: `${id}-form-item-description`,
    formMessageId: `${id}-form-item-message`,
    ...fieldState,
  }
}

type FormItemContextValue = {
  id: string
}

const FormItemContext = React.createContext<FormItemContextValue>(
  {} as FormItemContextValue
)

const FormItem = React.forwardRef<
  HTMLDivElement,
  React.HTMLAttributes<HTMLDivElement>
>(({ className, ...props }, ref) => {
  const id = React.useId()

  return (
    <FormItemContext.Provider value={{ id }}>
      <div ref={ref} className={cn("space-y-2", className)} {...props} />
    </FormItemContext.Provider>
  )
})
FormItem.displayName = "FormItem"

const FormLabel = React.forwardRef<
  React.ElementRef<typeof LabelPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof LabelPrimitive.Root>
>(({ className, ...props }, ref) => {
  const { error, formItemId } = useFormField()

  return (
    <Label
      ref={ref}
      className={cn(error && "text-destructive", className)}
      htmlFor={formItemId}
      {...props}
    />
  )
})
FormLabel.displayName = "FormLabel"

const FormControl = React.forwardRef<
  React.ElementRef<typeof Slot>,
  React.ComponentPropsWithoutRef<typeof Slot>
>(({ ...props }, ref) => {
  const { error, formItemId, formDescriptionId, formMessageId } = useFormField()

  return (
    <Slot
      ref={ref}
      id={formItemId}
      aria-describedby={
        !error
          ? `${formDescriptionId}`
          : `${formDescriptionId} ${formMessageId}`
      }
      aria-invalid={!!error}
      {...props}
    />
  )
})
FormControl.displayName = "FormControl"

const FormDescription = React.forwardRef<
  HTMLParagraphElement,
  React.HTMLAttributes<HTMLParagraphElement>
>(({ className, ...props }, ref) => {
  const { formDescriptionId } = useFormField()

  return (
    <p
      ref={ref}
      id={formDescriptionId}
      className={cn("text-[0.8rem] text-muted-foreground", className)}
      {...props}
    />
  )
})
FormDescription.displayName = "FormDescription"

const FormMessage = React.forwardRef<
  HTMLParagraphElement,
  React.HTMLAttributes<HTMLParagraphElement>
>(({ className, children, ...props }, ref) => {
  const { error, formMessageId } = useFormField()
  const body = error ? String(error?.message) : children

  if (!body) {
    return null
  }

  return (
    <p
      ref={ref}
      id={formMessageId}
      className={cn("text-[0.8rem] font-medium text-destructive", className)}
      {...props}
    >
      {body}
    </p>
  )
})
FormMessage.displayName = "FormMessage"

export {
  useFormField,
  Form,
  FormItem,
  FormLabel,
  FormControl,
  FormDescription,
  FormMessage,
  FormField,
}
````

## File: Frontend/src/components/ui/input.tsx
````typescript
import * as React from "react"

import { cn } from "@/lib/utils"

const Input = React.forwardRef<HTMLInputElement, React.ComponentProps<"input">>(
  ({ className, type, ...props }, ref) => {
    return (
      <input
        type={type}
        className={cn(
          "flex h-9 w-full rounded-md border border-input bg-transparent px-3 py-1 text-base shadow-sm transition-colors file:border-0 file:bg-transparent file:text-sm file:font-medium file:text-foreground placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 md:text-sm",
          className
        )}
        ref={ref}
        {...props}
      />
    )
  }
)
Input.displayName = "Input"

export { Input }
````

## File: Frontend/src/components/ui/label.tsx
````typescript
"use client"

import * as React from "react"
import * as LabelPrimitive from "@radix-ui/react-label"
import { cva, type VariantProps } from "class-variance-authority"

import { cn } from "@/lib/utils"

const labelVariants = cva(
  "text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70"
)

const Label = React.forwardRef<
  React.ElementRef<typeof LabelPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof LabelPrimitive.Root> &
    VariantProps<typeof labelVariants>
>(({ className, ...props }, ref) => (
  <LabelPrimitive.Root
    ref={ref}
    className={cn(labelVariants(), className)}
    {...props}
  />
))
Label.displayName = LabelPrimitive.Root.displayName

export { Label }
````

## File: Frontend/src/components/ui/popover.tsx
````typescript
"use client"

import * as React from "react"
import * as PopoverPrimitive from "@radix-ui/react-popover"

import { cn } from "@/lib/utils"

const Popover = PopoverPrimitive.Root

const PopoverTrigger = PopoverPrimitive.Trigger

const PopoverAnchor = PopoverPrimitive.Anchor

const PopoverContent = React.forwardRef<
  React.ElementRef<typeof PopoverPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof PopoverPrimitive.Content>
>(({ className, align = "center", sideOffset = 4, ...props }, ref) => (
  <PopoverPrimitive.Portal>
    <PopoverPrimitive.Content
      ref={ref}
      align={align}
      sideOffset={sideOffset}
      className={cn(
        "z-50 w-72 rounded-md border bg-popover p-4 text-popover-foreground shadow-md outline-none data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        className
      )}
      {...props}
    />
  </PopoverPrimitive.Portal>
))
PopoverContent.displayName = PopoverPrimitive.Content.displayName

export { Popover, PopoverTrigger, PopoverContent, PopoverAnchor }
````

## File: Frontend/src/components/ui/radio-group.tsx
````typescript
"use client"

import * as React from "react"
import * as RadioGroupPrimitive from "@radix-ui/react-radio-group"
import { Circle } from "lucide-react"

import { cn } from "@/lib/utils"

const RadioGroup = React.forwardRef<
  React.ElementRef<typeof RadioGroupPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof RadioGroupPrimitive.Root>
>(({ className, ...props }, ref) => {
  return (
    <RadioGroupPrimitive.Root
      className={cn("grid gap-2", className)}
      {...props}
      ref={ref}
    />
  )
})
RadioGroup.displayName = RadioGroupPrimitive.Root.displayName

const RadioGroupItem = React.forwardRef<
  React.ElementRef<typeof RadioGroupPrimitive.Item>,
  React.ComponentPropsWithoutRef<typeof RadioGroupPrimitive.Item>
>(({ className, ...props }, ref) => {
  return (
    <RadioGroupPrimitive.Item
      ref={ref}
      className={cn(
        "aspect-square h-4 w-4 rounded-full border border-primary text-primary shadow focus:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50",
        className
      )}
      {...props}
    >
      <RadioGroupPrimitive.Indicator className="flex items-center justify-center">
        <Circle className="h-3.5 w-3.5 fill-primary" />
      </RadioGroupPrimitive.Indicator>
    </RadioGroupPrimitive.Item>
  )
})
RadioGroupItem.displayName = RadioGroupPrimitive.Item.displayName

export { RadioGroup, RadioGroupItem }
````

## File: Frontend/src/components/ui/scroll-area.tsx
````typescript
"use client"

import * as React from "react"
import * as ScrollAreaPrimitive from "@radix-ui/react-scroll-area"

import { cn } from "@/lib/utils"

const ScrollArea = React.forwardRef<
  React.ElementRef<typeof ScrollAreaPrimitive.Root>,
  React.ComponentPropsWithoutRef<typeof ScrollAreaPrimitive.Root>
>(({ className, children, ...props }, ref) => (
  <ScrollAreaPrimitive.Root
    ref={ref}
    className={cn("relative overflow-hidden", className)}
    {...props}
  >
    <ScrollAreaPrimitive.Viewport className="h-full w-full rounded-[inherit]">
      {children}
    </ScrollAreaPrimitive.Viewport>
    <ScrollBar />
    <ScrollAreaPrimitive.Corner />
  </ScrollAreaPrimitive.Root>
))
ScrollArea.displayName = ScrollAreaPrimitive.Root.displayName

const ScrollBar = React.forwardRef<
  React.ElementRef<typeof ScrollAreaPrimitive.ScrollAreaScrollbar>,
  React.ComponentPropsWithoutRef<typeof ScrollAreaPrimitive.ScrollAreaScrollbar>
>(({ className, orientation = "vertical", ...props }, ref) => (
  <ScrollAreaPrimitive.ScrollAreaScrollbar
    ref={ref}
    orientation={orientation}
    className={cn(
      "flex touch-none select-none transition-colors",
      orientation === "vertical" &&
        "h-full w-2.5 border-l border-l-transparent p-[1px]",
      orientation === "horizontal" &&
        "h-2.5 flex-col border-t border-t-transparent p-[1px]",
      className
    )}
    {...props}
  >
    <ScrollAreaPrimitive.ScrollAreaThumb className="relative flex-1 rounded-full bg-border" />
  </ScrollAreaPrimitive.ScrollAreaScrollbar>
))
ScrollBar.displayName = ScrollAreaPrimitive.ScrollAreaScrollbar.displayName

export { ScrollArea, ScrollBar }
````

## File: Frontend/src/components/ui/select.tsx
````typescript
"use client"

import * as React from "react"
import * as SelectPrimitive from "@radix-ui/react-select"
import { Check, ChevronDown, ChevronUp } from "lucide-react"

import { cn } from "@/lib/utils"

const Select = SelectPrimitive.Root

const SelectGroup = SelectPrimitive.Group

const SelectValue = SelectPrimitive.Value

const SelectTrigger = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Trigger>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Trigger>
>(({ className, children, ...props }, ref) => (
  <SelectPrimitive.Trigger
    ref={ref}
    className={cn(
      "flex h-9 w-full items-center justify-between whitespace-nowrap rounded-md border border-input bg-transparent px-3 py-2 text-sm shadow-sm ring-offset-background placeholder:text-muted-foreground focus:outline-none focus:ring-1 focus:ring-ring disabled:cursor-not-allowed disabled:opacity-50 [&>span]:line-clamp-1",
      className
    )}
    {...props}
  >
    {children}
    <SelectPrimitive.Icon asChild>
      <ChevronDown className="h-4 w-4 opacity-50" />
    </SelectPrimitive.Icon>
  </SelectPrimitive.Trigger>
))
SelectTrigger.displayName = SelectPrimitive.Trigger.displayName

const SelectScrollUpButton = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.ScrollUpButton>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.ScrollUpButton>
>(({ className, ...props }, ref) => (
  <SelectPrimitive.ScrollUpButton
    ref={ref}
    className={cn(
      "flex cursor-default items-center justify-center py-1",
      className
    )}
    {...props}
  >
    <ChevronUp className="h-4 w-4" />
  </SelectPrimitive.ScrollUpButton>
))
SelectScrollUpButton.displayName = SelectPrimitive.ScrollUpButton.displayName

const SelectScrollDownButton = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.ScrollDownButton>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.ScrollDownButton>
>(({ className, ...props }, ref) => (
  <SelectPrimitive.ScrollDownButton
    ref={ref}
    className={cn(
      "flex cursor-default items-center justify-center py-1",
      className
    )}
    {...props}
  >
    <ChevronDown className="h-4 w-4" />
  </SelectPrimitive.ScrollDownButton>
))
SelectScrollDownButton.displayName =
  SelectPrimitive.ScrollDownButton.displayName

const SelectContent = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Content>
>(({ className, children, position = "popper", ...props }, ref) => (
  <SelectPrimitive.Portal>
    <SelectPrimitive.Content
      ref={ref}
      className={cn(
        "relative z-50 max-h-96 min-w-[8rem] overflow-hidden rounded-md border bg-popover text-popover-foreground shadow-md data-[state=open]:animate-in data-[state=closed]:animate-out data-[state=closed]:fade-out-0 data-[state=open]:fade-in-0 data-[state=closed]:zoom-out-95 data-[state=open]:zoom-in-95 data-[side=bottom]:slide-in-from-top-2 data-[side=left]:slide-in-from-right-2 data-[side=right]:slide-in-from-left-2 data-[side=top]:slide-in-from-bottom-2",
        position === "popper" &&
          "data-[side=bottom]:translate-y-1 data-[side=left]:-translate-x-1 data-[side=right]:translate-x-1 data-[side=top]:-translate-y-1",
        className
      )}
      position={position}
      {...props}
    >
      <SelectScrollUpButton />
      <SelectPrimitive.Viewport
        className={cn(
          "p-1",
          position === "popper" &&
            "h-[var(--radix-select-trigger-height)] w-full min-w-[var(--radix-select-trigger-width)]"
        )}
      >
        {children}
      </SelectPrimitive.Viewport>
      <SelectScrollDownButton />
    </SelectPrimitive.Content>
  </SelectPrimitive.Portal>
))
SelectContent.displayName = SelectPrimitive.Content.displayName

const SelectLabel = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Label>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Label>
>(({ className, ...props }, ref) => (
  <SelectPrimitive.Label
    ref={ref}
    className={cn("px-2 py-1.5 text-sm font-semibold", className)}
    {...props}
  />
))
SelectLabel.displayName = SelectPrimitive.Label.displayName

const SelectItem = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Item>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Item>
>(({ className, children, ...props }, ref) => (
  <SelectPrimitive.Item
    ref={ref}
    className={cn(
      "relative flex w-full cursor-default select-none items-center rounded-sm py-1.5 pl-2 pr-8 text-sm outline-none focus:bg-accent focus:text-accent-foreground data-[disabled]:pointer-events-none data-[disabled]:opacity-50",
      className
    )}
    {...props}
  >
    <span className="absolute right-2 flex h-3.5 w-3.5 items-center justify-center">
      <SelectPrimitive.ItemIndicator>
        <Check className="h-4 w-4" />
      </SelectPrimitive.ItemIndicator>
    </span>
    <SelectPrimitive.ItemText>{children}</SelectPrimitive.ItemText>
  </SelectPrimitive.Item>
))
SelectItem.displayName = SelectPrimitive.Item.displayName

const SelectSeparator = React.forwardRef<
  React.ElementRef<typeof SelectPrimitive.Separator>,
  React.ComponentPropsWithoutRef<typeof SelectPrimitive.Separator>
>(({ className, ...props }, ref) => (
  <SelectPrimitive.Separator
    ref={ref}
    className={cn("-mx-1 my-1 h-px bg-muted", className)}
    {...props}
  />
))
SelectSeparator.displayName = SelectPrimitive.Separator.displayName

export {
  Select,
  SelectGroup,
  SelectValue,
  SelectTrigger,
  SelectContent,
  SelectLabel,
  SelectItem,
  SelectSeparator,
  SelectScrollUpButton,
  SelectScrollDownButton,
}
````

## File: Frontend/src/components/ui/table.tsx
````typescript
import * as React from "react"

import { cn } from "@/lib/utils"

const Table = React.forwardRef<
  HTMLTableElement,
  React.HTMLAttributes<HTMLTableElement>
>(({ className, ...props }, ref) => (
  <div className="relative w-full overflow-auto">
    <table
      ref={ref}
      className={cn("w-full caption-bottom text-sm", className)}
      {...props}
    />
  </div>
))
Table.displayName = "Table"

const TableHeader = React.forwardRef<
  HTMLTableSectionElement,
  React.HTMLAttributes<HTMLTableSectionElement>
>(({ className, ...props }, ref) => (
  <thead ref={ref} className={cn("[&_tr]:border-b", className)} {...props} />
))
TableHeader.displayName = "TableHeader"

const TableBody = React.forwardRef<
  HTMLTableSectionElement,
  React.HTMLAttributes<HTMLTableSectionElement>
>(({ className, ...props }, ref) => (
  <tbody
    ref={ref}
    className={cn("[&_tr:last-child]:border-0", className)}
    {...props}
  />
))
TableBody.displayName = "TableBody"

const TableFooter = React.forwardRef<
  HTMLTableSectionElement,
  React.HTMLAttributes<HTMLTableSectionElement>
>(({ className, ...props }, ref) => (
  <tfoot
    ref={ref}
    className={cn(
      "border-t bg-muted/50 font-medium [&>tr]:last:border-b-0",
      className
    )}
    {...props}
  />
))
TableFooter.displayName = "TableFooter"

const TableRow = React.forwardRef<
  HTMLTableRowElement,
  React.HTMLAttributes<HTMLTableRowElement>
>(({ className, ...props }, ref) => (
  <tr
    ref={ref}
    className={cn(
      "border-b transition-colors hover:bg-muted/50 data-[state=selected]:bg-muted",
      className
    )}
    {...props}
  />
))
TableRow.displayName = "TableRow"

const TableHead = React.forwardRef<
  HTMLTableCellElement,
  React.ThHTMLAttributes<HTMLTableCellElement>
>(({ className, ...props }, ref) => (
  <th
    ref={ref}
    className={cn(
      "h-10 px-2 text-left align-middle font-medium text-muted-foreground [&:has([role=checkbox])]:pr-0 [&>[role=checkbox]]:translate-y-[2px]",
      className
    )}
    {...props}
  />
))
TableHead.displayName = "TableHead"

const TableCell = React.forwardRef<
  HTMLTableCellElement,
  React.TdHTMLAttributes<HTMLTableCellElement>
>(({ className, ...props }, ref) => (
  <td
    ref={ref}
    className={cn(
      "p-2 align-middle [&:has([role=checkbox])]:pr-0 [&>[role=checkbox]]:translate-y-[2px]",
      className
    )}
    {...props}
  />
))
TableCell.displayName = "TableCell"

const TableCaption = React.forwardRef<
  HTMLTableCaptionElement,
  React.HTMLAttributes<HTMLTableCaptionElement>
>(({ className, ...props }, ref) => (
  <caption
    ref={ref}
    className={cn("mt-4 text-sm text-muted-foreground", className)}
    {...props}
  />
))
TableCaption.displayName = "TableCaption"

export {
  Table,
  TableHeader,
  TableBody,
  TableFooter,
  TableHead,
  TableRow,
  TableCell,
  TableCaption,
}
````

## File: Frontend/src/components/ui/tabs.tsx
````typescript
"use client"

import * as React from "react"
import * as TabsPrimitive from "@radix-ui/react-tabs"

import { cn } from "@/lib/utils"

const Tabs = TabsPrimitive.Root

const TabsList = React.forwardRef<
  React.ElementRef<typeof TabsPrimitive.List>,
  React.ComponentPropsWithoutRef<typeof TabsPrimitive.List>
>(({ className, ...props }, ref) => (
  <TabsPrimitive.List
    ref={ref}
    className={cn(
      "inline-flex h-9 items-center justify-center rounded-lg bg-muted p-1 text-muted-foreground",
      className
    )}
    {...props}
  />
))
TabsList.displayName = TabsPrimitive.List.displayName

const TabsTrigger = React.forwardRef<
  React.ElementRef<typeof TabsPrimitive.Trigger>,
  React.ComponentPropsWithoutRef<typeof TabsPrimitive.Trigger>
>(({ className, ...props }, ref) => (
  <TabsPrimitive.Trigger
    ref={ref}
    className={cn(
      "inline-flex items-center justify-center whitespace-nowrap rounded-md px-3 py-1 text-sm font-medium ring-offset-background transition-all focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 data-[state=active]:bg-background data-[state=active]:text-foreground data-[state=active]:shadow",
      className
    )}
    {...props}
  />
))
TabsTrigger.displayName = TabsPrimitive.Trigger.displayName

const TabsContent = React.forwardRef<
  React.ElementRef<typeof TabsPrimitive.Content>,
  React.ComponentPropsWithoutRef<typeof TabsPrimitive.Content>
>(({ className, ...props }, ref) => (
  <TabsPrimitive.Content
    ref={ref}
    className={cn(
      "mt-2 ring-offset-background focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2",
      className
    )}
    {...props}
  />
))
TabsContent.displayName = TabsPrimitive.Content.displayName

export { Tabs, TabsList, TabsTrigger, TabsContent }
````

## File: Frontend/src/components/ui/textarea.tsx
````typescript
import * as React from "react"

import { cn } from "@/lib/utils"

const Textarea = React.forwardRef<
  HTMLTextAreaElement,
  React.ComponentProps<"textarea">
>(({ className, ...props }, ref) => {
  return (
    <textarea
      className={cn(
        "flex min-h-[60px] w-full rounded-md border border-input bg-transparent px-3 py-2 text-base shadow-sm placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-1 focus-visible:ring-ring disabled:cursor-not-allowed disabled:opacity-50 md:text-sm",
        className
      )}
      ref={ref}
      {...props}
    />
  )
})
Textarea.displayName = "Textarea"

export { Textarea }
````

## File: Frontend/src/components/ui/toast.tsx
````typescript
"use client"

import * as React from "react"
import * as ToastPrimitives from "@radix-ui/react-toast"
import { cva, type VariantProps } from "class-variance-authority"
import { X } from "lucide-react"

import { cn } from "@/lib/utils"

const ToastProvider = ToastPrimitives.Provider

const ToastViewport = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Viewport>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Viewport>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Viewport
    ref={ref}
    className={cn(
      "fixed top-0 z-[100] flex max-h-screen w-full flex-col-reverse p-4 sm:bottom-0 sm:right-0 sm:top-auto sm:flex-col md:max-w-[420px]",
      className
    )}
    {...props}
  />
))
ToastViewport.displayName = ToastPrimitives.Viewport.displayName

const toastVariants = cva(
  "group pointer-events-auto relative flex w-full items-center justify-between space-x-2 overflow-hidden rounded-md border p-4 pr-6 shadow-lg transition-all data-[swipe=cancel]:translate-x-0 data-[swipe=end]:translate-x-[var(--radix-toast-swipe-end-x)] data-[swipe=move]:translate-x-[var(--radix-toast-swipe-move-x)] data-[swipe=move]:transition-none data-[state=open]:animate-in data-[state=closed]:animate-out data-[swipe=end]:animate-out data-[state=closed]:fade-out-80 data-[state=closed]:slide-out-to-right-full data-[state=open]:slide-in-from-top-full data-[state=open]:sm:slide-in-from-bottom-full",
  {
    variants: {
      variant: {
        default: "border bg-background text-foreground",
        destructive:
          "destructive group border-destructive bg-destructive text-destructive-foreground",
      },
    },
    defaultVariants: {
      variant: "default",
    },
  }
)

const Toast = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Root>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Root> &
    VariantProps<typeof toastVariants>
>(({ className, variant, ...props }, ref) => {
  return (
    <ToastPrimitives.Root
      ref={ref}
      className={cn(toastVariants({ variant }), className)}
      {...props}
    />
  )
})
Toast.displayName = ToastPrimitives.Root.displayName

const ToastAction = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Action>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Action>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Action
    ref={ref}
    className={cn(
      "inline-flex h-8 shrink-0 items-center justify-center rounded-md border bg-transparent px-3 text-sm font-medium transition-colors hover:bg-secondary focus:outline-none focus:ring-1 focus:ring-ring disabled:pointer-events-none disabled:opacity-50 group-[.destructive]:border-muted/40 group-[.destructive]:hover:border-destructive/30 group-[.destructive]:hover:bg-destructive group-[.destructive]:hover:text-destructive-foreground group-[.destructive]:focus:ring-destructive",
      className
    )}
    {...props}
  />
))
ToastAction.displayName = ToastPrimitives.Action.displayName

const ToastClose = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Close>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Close>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Close
    ref={ref}
    className={cn(
      "absolute right-1 top-1 rounded-md p-1 text-foreground/50 opacity-0 transition-opacity hover:text-foreground focus:opacity-100 focus:outline-none focus:ring-1 group-hover:opacity-100 group-[.destructive]:text-red-300 group-[.destructive]:hover:text-red-50 group-[.destructive]:focus:ring-red-400 group-[.destructive]:focus:ring-offset-red-600",
      className
    )}
    toast-close=""
    {...props}
  >
    <X className="h-4 w-4" />
  </ToastPrimitives.Close>
))
ToastClose.displayName = ToastPrimitives.Close.displayName

const ToastTitle = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Title>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Title>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Title
    ref={ref}
    className={cn("text-sm font-semibold [&+div]:text-xs", className)}
    {...props}
  />
))
ToastTitle.displayName = ToastPrimitives.Title.displayName

const ToastDescription = React.forwardRef<
  React.ElementRef<typeof ToastPrimitives.Description>,
  React.ComponentPropsWithoutRef<typeof ToastPrimitives.Description>
>(({ className, ...props }, ref) => (
  <ToastPrimitives.Description
    ref={ref}
    className={cn("text-sm opacity-90", className)}
    {...props}
  />
))
ToastDescription.displayName = ToastPrimitives.Description.displayName

type ToastProps = React.ComponentPropsWithoutRef<typeof Toast>

type ToastActionElement = React.ReactElement<typeof ToastAction>

export {
  type ToastProps,
  type ToastActionElement,
  ToastProvider,
  ToastViewport,
  Toast,
  ToastTitle,
  ToastDescription,
  ToastClose,
  ToastAction,
}
````

## File: Frontend/src/components/ui/toaster.tsx
````typescript
"use client"

import { useToast } from "@/hooks/use-toast"
import {
  Toast,
  ToastClose,
  ToastDescription,
  ToastProvider,
  ToastTitle,
  ToastViewport,
} from "@/components/ui/toast"

export function Toaster() {
  const { toasts } = useToast()

  return (
    <ToastProvider>
      {toasts.map(function ({ id, title, description, action, ...props }) {
        return (
          <Toast key={id} {...props}>
            <div className="grid gap-1">
              {title && <ToastTitle>{title}</ToastTitle>}
              {description && (
                <ToastDescription>{description}</ToastDescription>
              )}
            </div>
            {action}
            <ToastClose />
          </Toast>
        )
      })}
      <ToastViewport />
    </ToastProvider>
  )
}
````

## File: Frontend/src/components/UserProfile.tsx
````typescript
// /app/profile/UserProfile.tsx
import React from "react";
import { UserCircleIcon } from "@heroicons/react/24/solid";

interface UserProfileProps {
  userData: {
    fullName: string;
    DOB: string;
    phoneNo: string;
    email: string;
    roleId: number;
    role: string;
    alreadyInCanada?: boolean | null;
    statusInCanada?: string | null;
    countryOfOrigin?: string | null;
    currentLocation?: string | null;
  };
}

const UserProfile: React.FC<UserProfileProps> = ({ userData }) => {
  return (
    <div className="max-w-5xl  mx-auto grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-20">
      {/* Card 1 - Profile Section */}
      <div className="bg-white shadow-md rounded-lg overflow-hidden">
        <div className="bg-gradient-to-r from-blue-600 to-blue-400 p-6 flex flex-col justify-center items-center text-white">
          <UserCircleIcon className="w-24 h-24 mb-4" />
          <h2 className="text-xl font-bold">{userData.fullName}</h2>
          <p className="text-sm">{userData.role.name}</p>
        </div>
        <div className="p-6 text-center">
          <p className="text-gray-600 font-semibold">Date of Birth</p>
          <p className="text-gray-600 text-center">
            {new Date(userData.DOB).toLocaleDateString()}
          </p>
          <p className="text-gray-600 font-semibold mt-4">Phone Number</p>
          <p className="text-gray-600 text-center">{userData.phoneNo}</p>
        </div>
      </div>

      {/* Card 2 - Email and Status */}
      <div className="bg-white shadow-md rounded-lg p-6">
        <div className="mt-12">
          <h3 className="text-lg text-center font-bold mb-4">
            Additional Information
          </h3>
          {userData.roleId === 1 && (
            <>
              <div className="mb-4">
                <p className="text-gray-600 text-center font-semibold">Email</p>
                <p className="text-gray-600 text-center">{userData.email}</p>
              </div>
              <div className="mb-4">
                <p className="text-gray-600 text-center font-semibold">
                  Already In Canada
                </p>
                <p className="text-gray-600 text-center">
                  {userData.alreadyInCanada ? "Yes" : "No"}
                </p>
              </div>
              {userData.alreadyInCanada && (
                <div className="mb-4">
                  <p className="text-gray-600 text-center font-semibold">
                    Status In Canada
                  </p>
                  <p className="text-gray-600 text-center">
                    {userData.statusInCanada || "N/A"}
                  </p>
                </div>
              )}
            </>
          )}
        </div>
      </div>

      {/* Card 3 - Country and Location */}
      <div className="bg-white shadow-md rounded-lg p-6">
        <div className="mt-14">
          <h3 className="text-lg text-center font-bold mb-4">
            Location Information
          </h3>
          {userData.roleId === 1 && (
            <>
              <div className="mb-4">
                <p className="text-gray-600 text-center font-semibold">
                  Country of Origin
                </p>
                <p className="text-gray-600 text-center">
                  {userData.countryOfOrigin || "N/A"}
                </p>
              </div>
              {userData.alreadyInCanada && (
                <div className="mb-4">
                  <p className="text-gray-600 text-center font-semibold">
                    School/Work Location
                  </p>
                  <p className="text-gray-600 text-center">
                    {userData.currentLocation || "N/A"}
                  </p>
                </div>
              )}
            </>
          )}
        </div>
      </div>
    </div>
  );
};

export default UserProfile;
````

## File: Frontend/src/hooks/use-toast.ts
````typescript
"use client"

// Inspired by react-hot-toast library
import * as React from "react"

import type {
  ToastActionElement,
  ToastProps,
} from "@/components/ui/toast"

const TOAST_LIMIT = 1
const TOAST_REMOVE_DELAY = 1000000

type ToasterToast = ToastProps & {
  id: string
  title?: React.ReactNode
  description?: React.ReactNode
  action?: ToastActionElement
}

const actionTypes = {
  ADD_TOAST: "ADD_TOAST",
  UPDATE_TOAST: "UPDATE_TOAST",
  DISMISS_TOAST: "DISMISS_TOAST",
  REMOVE_TOAST: "REMOVE_TOAST",
} as const

let count = 0

function genId() {
  count = (count + 1) % Number.MAX_SAFE_INTEGER
  return count.toString()
}

type ActionType = typeof actionTypes

type Action =
  | {
      type: ActionType["ADD_TOAST"]
      toast: ToasterToast
    }
  | {
      type: ActionType["UPDATE_TOAST"]
      toast: Partial<ToasterToast>
    }
  | {
      type: ActionType["DISMISS_TOAST"]
      toastId?: ToasterToast["id"]
    }
  | {
      type: ActionType["REMOVE_TOAST"]
      toastId?: ToasterToast["id"]
    }

interface State {
  toasts: ToasterToast[]
}

const toastTimeouts = new Map<string, ReturnType<typeof setTimeout>>()

const addToRemoveQueue = (toastId: string) => {
  if (toastTimeouts.has(toastId)) {
    return
  }

  const timeout = setTimeout(() => {
    toastTimeouts.delete(toastId)
    dispatch({
      type: "REMOVE_TOAST",
      toastId: toastId,
    })
  }, TOAST_REMOVE_DELAY)

  toastTimeouts.set(toastId, timeout)
}

export const reducer = (state: State, action: Action): State => {
  switch (action.type) {
    case "ADD_TOAST":
      return {
        ...state,
        toasts: [action.toast, ...state.toasts].slice(0, TOAST_LIMIT),
      }

    case "UPDATE_TOAST":
      return {
        ...state,
        toasts: state.toasts.map((t) =>
          t.id === action.toast.id ? { ...t, ...action.toast } : t
        ),
      }

    case "DISMISS_TOAST": {
      const { toastId } = action

      // ! Side effects ! - This could be extracted into a dismissToast() action,
      // but I'll keep it here for simplicity
      if (toastId) {
        addToRemoveQueue(toastId)
      } else {
        state.toasts.forEach((toast) => {
          addToRemoveQueue(toast.id)
        })
      }

      return {
        ...state,
        toasts: state.toasts.map((t) =>
          t.id === toastId || toastId === undefined
            ? {
                ...t,
                open: false,
              }
            : t
        ),
      }
    }
    case "REMOVE_TOAST":
      if (action.toastId === undefined) {
        return {
          ...state,
          toasts: [],
        }
      }
      return {
        ...state,
        toasts: state.toasts.filter((t) => t.id !== action.toastId),
      }
  }
}

const listeners: Array<(state: State) => void> = []

let memoryState: State = { toasts: [] }

function dispatch(action: Action) {
  memoryState = reducer(memoryState, action)
  listeners.forEach((listener) => {
    listener(memoryState)
  })
}

type Toast = Omit<ToasterToast, "id">

function toast({ ...props }: Toast) {
  const id = genId()

  const update = (props: ToasterToast) =>
    dispatch({
      type: "UPDATE_TOAST",
      toast: { ...props, id },
    })
  const dismiss = () => dispatch({ type: "DISMISS_TOAST", toastId: id })

  dispatch({
    type: "ADD_TOAST",
    toast: {
      ...props,
      id,
      open: true,
      onOpenChange: (open) => {
        if (!open) dismiss()
      },
    },
  })

  return {
    id: id,
    dismiss,
    update,
  }
}

function useToast() {
  const [state, setState] = React.useState<State>(memoryState)

  React.useEffect(() => {
    listeners.push(setState)
    return () => {
      const index = listeners.indexOf(setState)
      if (index > -1) {
        listeners.splice(index, 1)
      }
    }
  }, [state])

  return {
    ...state,
    toast,
    dismiss: (toastId?: string) => dispatch({ type: "DISMISS_TOAST", toastId }),
  }
}

export { useToast, toast }
````

## File: Frontend/src/lib/auth.ts
````typescript
import { cookies } from 'next/headers'

export async function getSession() {
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
  
  try {
    const cookieHeader = await cookies()
    const tokenResponse = await fetch(`${endpoint}auth/token`, {
      credentials: 'include',
      headers: {
        Cookie: cookieHeader.toString()
      }
    })
    
    if (!tokenResponse.ok) {
      return null
    }

    const tokenData = await tokenResponse.json()
    return tokenData.token ? { token: tokenData.token } : null
  } catch {
    return null
  }
}
````

## File: Frontend/src/lib/utils.ts
````typescript
import { clsx, type ClassValue } from "clsx"
import { twMerge } from "tailwind-merge"

export function cn(...inputs: ClassValue[]) {
  return twMerge(clsx(inputs))
}
````

## File: Frontend/src/middleware.ts
````typescript
import { NextResponse } from 'next/server'
import type { NextRequest } from 'next/server'

 
const publicRoutes = ['/', '/login', '/signup']
 
// Define role-based access control
const roleBasedAccess = {
  Admin: ['/dashboard/admin'],
  Immigrant: ['/dashboard/user'],
  Realtor: ['/dashboard/realtor'],
  CarDealership: ['/dashboard/car-dealer'],
  ImmigrationConsultant: ['/dashboard/consultant'],
  Onboarding: ['/onboarding'],
  NotVerified: ['/dashboard/not-verified']
}
 
export async function middleware(request: NextRequest) {
  const pathname = request.nextUrl.pathname
 
  // Skip public routes
  if (publicRoutes.includes(pathname)) {
    return NextResponse.next()
  }
 
  const endpoint = process.env.NEXT_PUBLIC_API_URL;
 
  try {
    const cookies = request.cookies
    const tokenResponse = await fetch(`${endpoint}auth/token`, {
      credentials: 'include',
      headers: {
        Cookie: cookies.toString(),
      },
    })
 
    if (!tokenResponse.ok) {
      return NextResponse.redirect(new URL('/login', request.url))
    }
 
    const tokenData = await tokenResponse.json()
    const token = tokenData.token
 
    if (!token) {
      return NextResponse.redirect(new URL('/login', request.url))
    }
    const roleName = tokenData.roleName.split(" ").join("");
    const allowedRoutes = roleBasedAccess[roleName] || []
 
    // Check if user is allowed to access this route
    const isAllowed = allowedRoutes.some(route => pathname.startsWith(route))
 
    if (!isAllowed) {
      return NextResponse.redirect(new URL('/unauthorized', request.url)) // or any fallback route
    }
 
    // Add token to request headers
    const requestHeaders = new Headers(request.headers)
    requestHeaders.set('Authorization', `Bearer ${token}`)
 
    return NextResponse.next({
      request: {
        headers: requestHeaders,
      },
    })
  } catch {
    return NextResponse.redirect(new URL('/', request.url))
  }
}
 
export const config = {
  matcher: [
    '/dashboard/:path*',
    '/onboarding/:path*',
  ],
}
````

## File: Frontend/tailwind.config.ts
````typescript
import type { Config } from "tailwindcss";
import animate from "tailwindcss-animate";

export default {
	darkMode: ["class"],
	content: [
		"./src/pages/**/*.{js,ts,jsx,tsx,mdx}",
		"./src/components/**/*.{js,ts,jsx,tsx,mdx}",
		"./src/app/**/*.{js,ts,jsx,tsx,mdx}",
	],
	theme: {
		extend: {
			colors: {
				background: 'hsl(var(--background))',
				foreground: 'hsl(var(--foreground))',
				card: {
					DEFAULT: 'hsl(var(--card))',
					foreground: 'hsl(var(--card-foreground))'
				},
				popover: {
					DEFAULT: 'hsl(var(--popover))',
					foreground: 'hsl(var(--popover-foreground))'
				},
				primary: {
					DEFAULT: 'hsl(var(--primary))',
					foreground: 'hsl(var(--primary-foreground))'
				},
				secondary: {
					DEFAULT: 'hsl(var(--secondary))',
					foreground: 'hsl(var(--secondary-foreground))'
				},
				muted: {
					DEFAULT: 'hsl(var(--muted))',
					foreground: 'hsl(var(--muted-foreground))'
				},
				accent: {
					DEFAULT: 'hsl(var(--accent))',
					foreground: 'hsl(var(--accent-foreground))'
				},
				destructive: {
					DEFAULT: 'hsl(var(--destructive))',
					foreground: 'hsl(var(--destructive-foreground))'
				},
				border: 'hsl(var(--border))',
				input: 'hsl(var(--input))',
				ring: 'hsl(var(--ring))',
				chart: {
					'1': 'hsl(var(--chart-1))',
					'2': 'hsl(var(--chart-2))',
					'3': 'hsl(var(--chart-3))',
					'4': 'hsl(var(--chart-4))',
					'5': 'hsl(var(--chart-5))'
				}
			},
			borderRadius: {
				lg: 'var(--radius)',
				md: 'calc(var(--radius) - 2px)',
				sm: 'calc(var(--radius) - 4px)'
			}
		}
	},
	plugins: [animate],
} satisfies Config;
````

## File: Frontend/tsconfig.json
````json
{
  "compilerOptions": {
    "target": "ES2017",
    "lib": ["dom", "dom.iterable", "esnext"],
    "allowJs": true,
    "skipLibCheck": true,
    "strict": true,
    "noEmit": true,
    "esModuleInterop": true,
    "module": "esnext",
    "moduleResolution": "bundler",
    "resolveJsonModule": true,
    "isolatedModules": true,
    "jsx": "preserve",
    "incremental": true,
    "plugins": [
      {
        "name": "next"
      }
    ],
    "paths": {
      "@/*": ["./src/*"]
    }
  },
  "include": ["next-env.d.ts", "**/*.ts", "**/*.tsx", ".next/types/**/*.ts"],
  "exclude": ["node_modules"]
}
````

## File: repomix.config.json
````json
{
  "output": {
    "filePath": "repomix-output.md",
    "style": "markdown",
    "parsableStyle": false,
    "fileSummary": true,
    "directoryStructure": true,
    "removeComments": false,
    "removeEmptyLines": false,
    "compress": false,
    "topFilesLength": 5,
    "showLineNumbers": false,
    "copyToClipboard": false,
    "git": {
      "sortByChanges": true,
      "sortByChangesMaxCommits": 100
    }
  },
  "include": [],
  "ignore": {
    "useGitignore": true,
    "useDefaultPatterns": true,
    "customPatterns": []
  },
  "security": {
    "enableSecurityCheck": true
  },
  "tokenCount": {
    "encoding": "o200k_base"
  }
}
````
