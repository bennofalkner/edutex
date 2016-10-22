# edutex

## deprecated in fovor of edo.tex (see https://github.com/bennof/edo.tex)

EduTeX is a document preparation system and document markup language using the TeX typesetting system for output. The system is focusing small disk space and pdf output for education.

EduTeX will be designed to perform stuff typically used for education. A major focus are worksheets, tests and classroom management. The advantage of TeX compared to MS Word and other office suites is the more accurate typsetting, mathematical formula setting and the programming language. 

In contrast to LaTeX EduTex will be used as indented by Knuth as a format file. This format file will be based on plainTeX and can be modified by several tools and scripts. This becomes important for portability. Today we are using more and more tablets i.e. Android. In that case disk space is limited and not all LaTeX packages can be added. To solve this problem EduTeX will use a default format file, which can be replaced by institute dependent settings. So everybody can use free documents for his institute and share their work on the web.Additional macros can be included in a document and are shared with the document.  

The basic idea is to create a folder instead of a single file like:

    someFile.etx/        (root folder)
      -> someFile.tex    (tex file)
      -> someFile.pdf    (pdf output generated by pdftex)
      -> data/           (data folder for images etc.)
      -> .tex/           (hidden folder - tex code / compatibility)
    
    
As folders are not easy to share a zipped file format will be introduced to:

    someFile.etxz and someFile.etx.zip
  (The second naming is for compatibility. Zip files are recognized and extracted automatically by the os.)

Currently - another file design is tested. Because TeX is not often used by ordinary users but PDF is well known, it seams to be an option to include zipped data in a PDF as an not referenced stream inside the PDF document. 
    
To be continued ...
