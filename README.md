# pymol-movie pymol 保存透明背景图片
# 鼠标操作：
1 open pse with pymol
2 click movie - program - camera loop - y-roll - 8seconds
# pymol命令行
set ray_opaque_background, off # 设置背景透明，详细介绍见 pymol wiki cmd.png()
新建pngs文件夹
iterate frames and save png with transparent backgrouond into folder
for i in range(1,241):cmd.frame(i),cmd.png('%03d.png'%i,width=800,height=800,dpi=300,ray=1)
