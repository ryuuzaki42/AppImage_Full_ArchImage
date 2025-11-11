# AppImage_Full_ArchImage

## AppImage with large size, but with more support
### For example with Glibc>=2.34 or QT6 inside.

### Check the recipes:
https://github.com/ryuuzaki42/AppImage_Full_ArchImage/tree/main/recipes

### Check the releases:
https://github.com/ryuuzaki42/AppImage_Full_ArchImage/releases

## Using ArchImage
https://github.com/ivan-hc/ArchImage

./archimage-cli -b prog

    blank
    blank
    y
    y

## Rename
```
file_name=$(ls *.AppImage)
file_name_new=$(echo "$file_name" | rev | cut -d '.' -f2- | rev)
file_name_new=$(echo "${file_name_new}-1_JB.AppImage")

echo "$file_name $file_name_new"

mv $file_name $file_name_new
md5sum $file_name_new > ${file_name_new}.md5

ls *AppImage*
```
---
Up 11/11/2025 - 02
