# TemplateRex
TemplateRex - A Template toolkit that partitions code from text and uses nestable sections.

# Synopsis 

Assuming you have the following:
1. Template file - "my_template.html"
2. Hash consisting of the data to merge with the template - %data_hsh

   use TemplateRex;

   $args{'file'} = "my_template.html";

   $t_rex = new TemplateRex( %args );            # Arguments can be either a hash or hash reference

   $t_rex->render(\%data_hsh);                   # Prints to standard out
   $t_rex->render(\%data_hsh, "rendered.html")   # Prints to a file

 
