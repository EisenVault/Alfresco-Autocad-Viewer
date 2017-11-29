#Previewing Autocad files (.dwg) files in Alfresco Share
This addon works with Alfresco 5.1 and 5.2. Please follow instructions below.

For installer > 5.1 apply Autocad_server_repo.amp . and follow these steps
1. Install the given trial package of qcad any version higer than this will show watermark on the document. it will get installed on /home/{user}/opt/qcad-3.17.3-trial-linux-x86_64
This correct version can be downloaded from: 

2. Update the alfresco-global.properties file by adding.

'''
dwg2pdf.root=/home/{user}//opt/qcad-3.17.3-trial-linux-x86_64
content.transformer.dwg2pdf.priority=50
content.transformer.dwg2pdf.extensions.dwg.pdf.supported=true
content.transformer.dwg2pdf.extensions.dwg.pdf.priority=50
content.transformer.dxf2pdf.priority=50
content.transformer.dxf2pdf.extensions.dxf.pdf.supported=true
content.transformer.dxf2pdf.extensions.dxf.pdf.priority=50
'''

#Authors & Attribution
Written by Tushar Khanka of EisenVault (www.eisenvault.com).

Write to us at: engineering@eisenvault.com

Code based on instructions written by Soft29 at: http://soft29.info/blog/entry/alfresco-cad-dxf-dwg-preview

Relies on QCAD community edition, itself released under GPL v3.0 (https://qcad.org/en/qcad-downloads-trial)
