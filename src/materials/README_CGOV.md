
<pre>
<h4 id="synopsis"><b>SYNOPSIS</b></h4><pre>       <b>gcovr</b> [<u>options</u>]

</pre><h4 id="description"><b>DESCRIPTION</b></h4><pre>       A utility to run gcov and generate a simple report that summarizes the coverage

</pre><h4 id="options"><b>OPTIONS</b></h4>
<pre>       <b>-h</b>, <b>--help</b>
              show this help message and exit

       <b>--version</b>
              Print the version number, then exit

       <b>-v</b>, <b>--verbose</b>
              Print progress messages

       <b>--object-directory</b>=<u>OBJDIR</u>
              Specify  the  directory  that  contains the gcov data files.  gcovr must be able to
              identify the path between  the  *.gcda  files  and  the  directory  where  gcc  was
              originally  run.   Normally,  gcovr  can  guess  correctly.   This option overrides
              gcovr's normal path detection and can specify either the path from gcc to the  gcda
              file (i.e. what was passed to gcc's '-o' option), or the path from the gcda file to
              gcc's original working directory.

       <b>-o</b> OUTPUT, <b>--output</b>=<u>OUTPUT</u>
              Print output to this filename

       <b>-k</b>, <b>--keep</b>
              Keep the temporary *.gcov files generated by gcov.  By default, these are deleted.

       <b>-d</b>, <b>--delete</b>
              Delete the coverage files after they are processed.  These  are  generated  by  the
              users's program, and by default gcovr does not remove these files.

       <b>-f</b> FILTER, <b>--filter</b>=<u>FILTER</u>
              Keep only the data files that match this regular expression

       <b>-e</b> EXCLUDE, <b>--exclude</b>=<u>EXCLUDE</u>
              Exclude data files that match this regular expression

       <b>--gcov-filter</b>=<u>GCOV_FILTER</u>
              Keep only gcov data files that match this regular expression

       <b>--gcov-exclude</b>=<u>GCOV_EXCLUDE</u>
              Exclude gcov data files that match this regular expression

       <b>-r</b> ROOT, <b>--root</b>=<u>ROOT</u>
              Defines  the  root  directory  for  source  files.  This is also used to filter the
              files, and to standardize the output.

       <b>-x</b>, <b>--xml</b>
              Generate XML instead of the normal tabular output.

       <b>--xml-pretty</b>
              Generate pretty XML instead of the normal dense format.

       <b>--html</b> Generate HTML instead of the normal tabular output.

       <b>--html-details</b>
              Generate HTML output for source file coverage.

       <b>--html-absolute-paths</b>
              Set the paths in the HTML report to be absolute instead of relative

       <b>-b</b>, <b>--branches</b>
              Tabulate the branch coverage instead of the line coverage.

       <b>-u</b>, <b>--sort-uncovered</b>
              Sort entries by increasing number of uncovered lines.

       <b>-p</b>, <b>--sort-percentage</b>
              Sort entries by decreasing percentage of covered lines.

       <b>--gcov-executable</b>=<u>GCOV_CMD</u>
              Defines the name/path to the gcov executable  [defaults  to  the  GCOV  environment
              variable, if present; else 'gcov'].

       <b>--exclude-unreachable-branches</b>
              Exclude from coverage branches which are marked to be excluded by LCOV/GCOV markers
              or are determined to be from lines containing only compiler-generated "dead" code.

       <b>--exclude-directories</b>=<u>EXCLUDE_DIRS</u>
              Exclude directories from search path that match this regular expression

       <b>-g</b>, <b>--use-gcov-files</b>
              Use preprocessed gcov files for analysis.

       <b>-s</b>, <b>--print-summary</b>
              Prints a small report to stdout with line &amp; branch percentage coverage

</pre>
<h4 id="copyright"><b>COPYRIGHT</b></h4>
<pre> 
    Copyright (2013) Sandia Corporation. Under the terms of  Contract  DE-AC04-94AL85000  with
    Sandia Corporation, the U.S. Government retains certain rights in this software.
</pre>
<div>
    <h4>SEE ALSO</h4>
    <p>     
        The full documentation for <b>gcovr</b> is maintained as a Texinfo manual.  
        If the <b>info</b> and <b>gcovr</b>
        programs are properly installed at your site, the command
    </p>
    <p>
        info gcovr -should give you access to the complete manual.
    </p>
</div>
