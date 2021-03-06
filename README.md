# TaskHelper-VBA-iSeries

*(Please note: this project is a work in progress.  This is being developed by only a single person, in a live environment, by someone fully committed to other, non-programming responsibilities.  Also because of these details, I may not always be able to maintain "best practices" throughout each iteration.)*

See the included LICENSE.md file for a copy of the GNU General Public License. 

## Version

**1.1**

## About

The **TaskHelper VBA iSeries** is a glue application built to automate processes performed between Microsoft Excel and IBM's AS/400.  The TaskHelper uses IBM's Host Access Class Library (HACL) and works exclusively through client-side access.

Because of its reliance on *GetText/SetText*, it only works "as is" within a single company's AS/400 implementation.  However, those individuals seeking to learn more about Excel-to-AS/400 automation may find the overall use of the HACL to be informative for their own purposes.

With each iteration of this project, I'll do what I can to localize context requirments, but I can't guarantee true *context-free code* for quite a long time, if at all.  This code is being uploaded to github.com due to our simple lack of version control.

To learn more about IBM's HACL:

http://www-01.ibm.com/support/knowledgecenter/SSEQ5Y_5.9.0/com.ibm.pcomm.doc/books/html/host_access06.htm

## Testing

**The TaskHelper assumes the client can create a new instance of the *autECLSession* object.**  This is a non-trivial 
concern for users on a thin-client or VPN, and a basic *"Set objAS400 = CreateObject("PCOMM.autECLSession")"*-style component test should be performed on workstations first so as to identify potential issues prior to real development.

## Module List

*To be added...*
