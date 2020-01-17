"# KB4534314--FAILED" 

we have patch many server and after reboot all 2008 serveurs not booting after install kb KB4534314

But, we have find solution for rollback in windows rescue mode this patch

When you are rescue mode find driver letter where you windows dir is installed 

for me i have c: and d:, in rescue mode c: is e:

If you need more information, you can use diskpart tools and when you have diskpart promt write list volume 

`dism /ScratchDir:e:\tmp\ /image:e:\ /remove-Package /PackageName:Package_for_KB4534314~31bf3856ad364e35~amd64~~6.1.1.9`

If you want win time download this iso image and mount this image

In rescue mode got to h: or f: and launch script

fore is your win dir is on e: 
forg is your win dir is on g:

etc etc  
