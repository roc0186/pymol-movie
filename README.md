# pymol
save pngs with transpatent background to make movie of Y-roll
# click ：
1 open pse with pymol

2 click movie - program - camera loop - y-roll - 8seconds
# pymol command
set ray_opaque_background, off # 设置背景透明，详细介绍见 pymol wiki cmd.png()

for i in range(1,241):cmd.frame(i),cmd.png('%03d.png'%i,width=800,height=800,dpi=300,ray=1) # make and go into folder 'pngs'，iterate frames and save png with transparent backgrouond into folder
