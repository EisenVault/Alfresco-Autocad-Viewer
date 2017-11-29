Previewing Autocad files (.dwg) files in alfresco share 5.2

For installer > 5.1 apply Autocad_server_repo.amp . and follow these steps
1. Install the given trial pakage of qcad any version higer than this will show watermark on the document. it will get installed on /home/{user}/opt/qcad-3.17.3-trial-linux-x86_64

2. Update the alfresco-global.properties file by adding.

## config for AutoCAD file viewing ###

dwg2pdf.root=/home/{user}//opt/qcad-3.17.3-trial-linux-x86_64
content.transformer.dwg2pdf.priority=50
content.transformer.dwg2pdf.extensions.dwg.pdf.supported=true
content.transformer.dwg2pdf.extensions.dwg.pdf.priority=50
content.transformer.dxf2pdf.priority=50
content.transformer.dxf2pdf.extensions.dxf.pdf.supported=true
content.transformer.dxf2pdf.extensions.dxf.pdf.priority=50

