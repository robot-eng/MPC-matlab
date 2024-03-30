# MPC-matlab
## Gain-Scheduled MPC Control of Nonlinear Chemical Reactor
**About the Continuous Stirred Tank Reactor**
<p>A continuously stirred tank reactor (CSTR) is a common chemical system in the process industry. A schematic of the CSTR system is:</p>

<p align="center"><img width="50%" src="/image/image.png" /></p>

<p>This system is a jacketed non-adiabatic tank reactor described extensively in [1]. The vessel is assumed to be perfectly mixed, and a single first-order exothermic and irreversible reaction, A --> B, takes place. The inlet stream of reagent A is fed to the tank at a constant volumetric rate. The product stream exits continuously at the same volumetric rate, and liquid density is constant. Thus, the volume of reacting liquid is constant.</p>
<p>The inputs of the CSTR model are:</p>

<p align="center"><img width="50%" src="/image/image-1.png" /></p>

<p>The outputs of the model, which are also the model states, are:</p>

<p align="center"><img width="50%" src="/image/image-2.png"></p>

### - Format Text in the Live Editor (file.mlx)
#### $\color{orange}{Insert \space Text \space Items}$
<p>To insert a new item, go to the Insert tab and select from the available options.</p>

| **Option** | **Description** | **Additional Details** |
|:--------:|:-------------|:--------------------|
|`Code`|Insert a blank line of code.|You can insert a code line before, after, or between text lines.|
|`Section Break`|Insert a section break.|You can insert a section break to divide your live script or function into manageable sections to evaluate individually. A section can consist of code, text, and output. For more information, see Create and Run Sections in Code.|
| `Text`  |    Insert a blank line of text.         |     A text line can contain formatted text, hyperlinks, images, or equations. You can insert a text line before, after, or between code lines.               |
|   `Table of Contents`     |      Insert a table of contents.       |  The table of contents contains a list of all the titles and headings in the document. If the document contains only one title, then it is not included in the table of contents. Only the title of the table of contents is editable. You can insert a table of contents only in text lines. If you insert a table of contents into a code line, MATLAB® places it directly above the current code section. When exporting a live script containing a table of contents to Microsoft® Word, by default, the table of contents in the resulting document does not include page numbers. To add page numbers, click the table of contents and select Update Table.              |
|    `Code Example`    |   Insert a formatted code example.          |      A code example is sample code that appears as indented and monospaced text.`Select Plain to insert sample code as unhighlighted text.` ` Select MATLAB to insert sample code as text highlighted according to MATLAB syntax.`              |
|   `Table`     |   Insert a table.          |       You can insert tables only in text lines. If you insert a table into a code line, MATLAB places the table in a new text line directly under the selected code line. To specify the table size, select Table drop-down arrow, move the cursor over the grid to highlight the numbers of rows and columns you want, and click to add the table. To create a larger table, click the table button , and specify the numbers of rows and columns in the dialog box. After inserting the table, you can modify its rows and columns: `Insert or delete rows and columns` - Right-click the table, select **Table**, and then select from the available insertion and deletion options. `Resize columns` - Click and drag the edge of the column. To reset the column widths, right-click and select **Table** > **Reset Column Widths**. `Make the first row a header row` - Right-click the table and select **Table** > **Turn Header Row On.**             |
|Image   |      Insert an image.       |         You can insert images only in text lines. If you insert an image into a code line, MATLAB places the image in a new text line directly under the selected code line. To change the alternate text, alignment, and size of an image after inserting it, right-click the image and select Edit Image... from the context menu. `Alt Text` - Add text to the edit field to specify alternative text for the image. `Alignment` - Select from the available options to specify how the image aligns with the other items in the row. `Size` - To specify a size relative to the original image size, select Relative (%) and specify the width and height of the image as a percentage of the original image. To specify an absolute size, select Absolute (px) and specify the width and height of the image in pixels. Select Keep Aspect Ratio to maintain the aspect ratio while resizing. `To return to the original image size, right-click the image and select Reset Image.`           |
|Hyperlink    |    Insert a hyperlink.         |           You can insert hyperlinks only in text lines. If you insert a hyperlink into a code line, MATLAB places the hyperlink in a new text line directly under the selected code line.`Select Web page to insert a hyperlink to an external web page. Then, enter the URL of the web page.` `Select Location in existing document to insert a hyperlink to a specific location in a separate live script or live function. Enter or browse for the file path and then select a location in the document preview that displays on the right.``Select Location in this document to insert a hyperlink that points to an existing location within the document. When prompted, click the desired location within the document to select it as the target. You also can use the Alt + Up Arrow and Alt + Down Arrow keyboard shortcuts. Location can be a code section, text paragraph, title, or heading. Linking to individual lines of text or code is not supported.``Select Existing file to insert a hyperlink to a file. Then, enter the file path.`         |
|      Equation   |       	Insert an equation.      |            You insert add equations only in text lines. If you insert an equation into a code line, MATLAB places the equation in a new text line directly under the selected code line. For more information, see Insert Equations into the Live Editor. |

#### $\color{orange}{Format \space Text}$
To format existing text, use any of the options included in the Live Editor tab Text section:

|    **Format Type**    |   **Options**          |      
|:------:|:------------|              
|   Text Style     |         Normal, Heading 1, Heading 2, Heading 3, Title     |                    
|    Text Alignment    |        Align left, Align center, Align right      |                    
|    Lists    |       Numbered list, Bulleted list       |                    
|    Standard Formatting    |        Bold, Italic, Underline, Monospaced      |  

#### $\color{orange}{Autoformatting}$

|    **Formatting Style**    |   **Autoformatting Sequence**          | **Keyboard Shortcut**|     
|:------:|:------------|:------------|               
|   Title     |        # text + **Enter**    |   **Ctrl + Alt + L**   |              
|   Heading 1    |        ## text + **Enter**    |   **Ctrl + Shift + 1**   | 
|   Heading 2   |        ### text + **Enter**    |   **Ctrl + Shift + 2**   | 
|   Heading 3    |        #### text + **Enter**    |   **Ctrl + Shift + 3**   | 
|   Section break with heading 1   |        %% text + **Enter**    |  With cursor at beginning of line with *text*: **Ctrl + Shift + 1**, then **Ctrl + Alt + Enter**    | 
|   Section break   |        %% + **Enter**, --- + **Enter**, *** + **Enter**    |   **CCtrl + Alt + Enter**   |
|   Bulleted list    |       * text, - text, + text    |   **Ctrl + Alt + U**   |
|   Numbered list   |        *number.* *text*    |   **Ctrl + Alt + O**   |
|   Italic   |        * ***text*** *, _ text _    |   **Ctrl + I**   |
|   Bold and italic  |        *** text ***, ___ text ___    |   **Ctrl + B**, then **Ctrl + I**   |
|   Bold   |        ** text **, __ text __    |   **Ctrl + B**   |
|   Monospace   |        `` `text` ``    |   **Ctrl + M**   |
|   Underline  |        None    |   **Ctrl + U**   |
|   LaTeX equation  |        $ LaTeX $    |   **Ctrl + Shift + L**   |
|   Hyperlink  |        URL + Space or Enter <URL>   |   **Ctrl + K**   |
|   Trademark, service mark, and copyright symbols (™, ℠, ®, and ©) | (TM), (SM), (R), (C)| None|