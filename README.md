# convert2poptree
Convert locus data in excel format to Poptree2 software

There are lots of software that measures of the extent of genetic differentiation between populations and constructs phylogenetic trees. Poptree2 is one of them, you can download and run Windows version: http://www.med.kagawa-u.ac.jp/~genomelb/takezaki/poptree2/index.html

If you have allele frequencies of different populations, you need to supply them to program in a specific format: http://www.med.kagawa-u.ac.jp/~genomelb/takezaki/poptree2/test.html

Most of data is already recorded in spreadsheets by scientists. You can use this small javascript code to load data in csv format and paste it to a poptree2 formatted text file. If you have locus names, you can tick the box "Locus name instead of locus sequence" before converting data. Poptree2 formated population names must not contain spaces because population names separated by spaces. So program replaces spaces (" ") with dashes "-".

You can copy/paste phylogenetic tree or save "nwk" format from Poptree2 software. You can also save calculations.

Steps to use that software

    1- You have HLA data entered to the file "demo-input.xlsx".
    2- Export "demo-input.xlsx" file as csv formatted "demo-input.csv" file
    3- Use "convert2poptree.js", choose "demo-input.csv" file, click "Read" to read it,
    4- Tick "Locus name instead of locus sequence", 
    5- Click "Convert"
    6- Click "Copy" to copy poptree2 formatted data to clipboard
    7- create a text file named "demo-output.dat", open it with a text editor, paste it, then save it. 
    8- instead of (6-7) you can use save button if your browser is compatible
    9- Download and run Poptree2 software, click "Data Input" to read "demo-output.dat". 
    10- Use poptree2 software.

You can use http://etetoolkit.org/treeview/ to paste "nwk" formatted text and draw phylogenetic tree. You can find example output at: http://etetoolkit.org/treeview/?treeid=3e0fa6820dcdf29e71533776a2a6ec21&algid= Click to "View tree!" to see the drawing

Note frequency data is real, and got from http://allelefrequencies.net
