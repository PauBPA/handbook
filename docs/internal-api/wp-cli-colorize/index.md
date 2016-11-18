---
layout: default
title: WP_CLI::colorize()
description: "Colorize a string for output."
---

<small><a href="/docs/">Docs</a> &raquo; <a href="/docs/internal-api/">Internal API</a> &raquo; Output</small>

## WP_CLI::colorize()

Colorize a string for output.

***

### Usage

    WP_CLI::colorize( $string )

<div>
<strong>$string</strong> (string) String to colorize for output, with color tokens.<br />
<strong>@return</strong> (string) string.<br />
</div>


***

### Notes

Yes, you too can change the color of command line text. For instance,
here's how `WP_CLI::success()` colorizes "Success: "


    WP_CLI::colorize( "%GSuccess:%n " )
    

Uses `\cli\Colors::colorize()` to transform color tokens to display
settings. Choose from the following tokens (and note 'reset'):

* %y => ['color' => 'yellow'],
* %g => ['color' => 'green'],
* %b => ['color' => 'blue'],
* %r => ['color' => 'red'],
* %p => ['color' => 'magenta'],
* %m => ['color' => 'magenta'],
* %c => ['color' => 'cyan'],
* %w => ['color' => 'grey'],
* %k => ['color' => 'black'],
* %n => ['color' => 'reset'],
* %Y => ['color' => 'yellow', 'style' => 'bright'],
* %G => ['color' => 'green', 'style' => 'bright'],
* %B => ['color' => 'blue', 'style' => 'bright'],
* %R => ['color' => 'red', 'style' => 'bright'],
* %P => ['color' => 'magenta', 'style' => 'bright'],
* %M => ['color' => 'magenta', 'style' => 'bright'],
* %C => ['color' => 'cyan', 'style' => 'bright'],
* %W => ['color' => 'grey', 'style' => 'bright'],
* %K => ['color' => 'black', 'style' => 'bright'],
* %N => ['color' => 'reset', 'style' => 'bright'],
* %3 => ['background' => 'yellow'],
* %2 => ['background' => 'green'],
* %4 => ['background' => 'blue'],
* %1 => ['background' => 'red'],
* %5 => ['background' => 'magenta'],
* %6 => ['background' => 'cyan'],
* %7 => ['background' => 'grey'],
* %0 => ['background' => 'black'],
* %F => ['style' => 'blink'],
* %U => ['style' => 'underline'],
* %8 => ['style' => 'inverse'],
* %9 => ['style' => 'bright'],
* %_ => ['style' => 'bright')


*Internal API documentation is generated from the WP-CLI codebase on every release. To suggest improvements, please submit a pull request.*


***

### Related

<ul>



<li><strong><a href="/docs/internal-api/wp-cli-utils-format-items/">WP_CLI\Utils\format_items()</a></strong> - Render a collection of items as an ASCII table, JSON, CSV, YAML, list of ids, or count.</li>


<li><strong><a href="/docs/internal-api/wp-cli-utils-make-progress-bar/">WP_CLI\Utils\make_progress_bar()</a></strong> - Create a progress bar to display percent completion of a given operation.</li>


<li><strong><a href="/docs/internal-api/wp-cli-line/">WP_CLI::line()</a></strong> - Display informational message without prefix, and ignore `--quiet`.</li>


<li><strong><a href="/docs/internal-api/wp-cli-log/">WP_CLI::log()</a></strong> - Display informational message without prefix.</li>


<li><strong><a href="/docs/internal-api/wp-cli-success/">WP_CLI::success()</a></strong> - Display success message prefixed with &quot;Success: &quot;.</li>


<li><strong><a href="/docs/internal-api/wp-cli-debug/">WP_CLI::debug()</a></strong> - Display debug message prefixed with &quot;Debug: &quot; when `--debug` is used.</li>


<li><strong><a href="/docs/internal-api/wp-cli-warning/">WP_CLI::warning()</a></strong> - Display warning message prefixed with &quot;Warning: &quot;.</li>


<li><strong><a href="/docs/internal-api/wp-cli-error/">WP_CLI::error()</a></strong> - Display error message prefixed with &quot;Error: &quot; and exit script.</li>


<li><strong><a href="/docs/internal-api/wp-cli-error-multi-line/">WP_CLI::error_multi_line()</a></strong> - Display a multi-line error message in a red box. Doesn't exit script.</li>



</ul>

