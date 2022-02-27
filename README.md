I found it odd that such a minimalist C program that can be only configured trough the source code needs an external program for displaying a custom bar via `xsetroot -name`, so to solve the issue I just made the bar in dwm.c

The patch file that I provided adds a few example bar "modules": load average, CPU temperature and time.
![image](https://user-images.githubusercontent.com/49120638/155901505-35764718-950e-441d-b8b1-e73433b1c94a.png)

To apply the patch enter the dwm directory then:
`patch -p1 < /path/to/dwm_internal_bar.diff`
