plover_dict_converter
=====================

A script to convert an RTF/CRE dictionary to a plover dictionary.

Eventually, this may be added to plover itself so it can directly load the dictionary.

This script relies on PLY: http://www.dabeaz.com/ply/

The script is invoked as:

python convert_rtfcre_to_json_dict.py <input rtf file> > output_dict.json 2> report.txt

Make sure to read the report.

To merge multiple plover dictionaries into one use the merge script. This will produce a dictionary where the later dictionaries override the earlier ones.

It is invoked as follows:
python merge_dicts.py dict1.json dict2.json ... > merged_dict.json 2> report.txt

You may want to see the report (or not).

There is also a script to convert from a plover json dictionary to an RTF/CRE dictionary that, in theory, could be imported by any other CAT program.

Make sure the command line is correct because the output file will be overwritten without warning:
python convert_json_to_rtfcre_dict.py <input json file> <output rtf file>

This is a first draft and needs some cleanup and improvement in usability.
