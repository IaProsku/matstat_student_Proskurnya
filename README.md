# myrepo
У цьому каталозі містяться лабораторні роботи з навчальної дисципліни
	«Алгоритми і методи обчислень» студента групи КІ-23-1 Проскурні Іллі


conky.config = {
    use_xft = true,
    font = 'DejaVu Sans Mono:size=10',
    update_interval = 1,
    own_window = true,
    own_window_type = 'desktop',
    own_window_transparent = true,
    own_window_hints = 'undecorated,below,sticky,skip_taskbar,skip_pager',
    double_buffer = true,
    minimum_width = 200, minimum_height = 200,
    alignment = 'top_right',
    gap_x = 20,
    gap_y = 60,
    default_color = 'white'
}

conky.text = [[
${font DejaVu Sans Mono:bold:size=12}System Monitor${font}
CPU: ${cpu}% ${alignr}Temp: ${hwmon temp 1}°C
RAM: $mem / $memmax ${alignr}Usage: $memperc%
GPU Temp: ${exec nvidia-smi --query-gpu=temperature.gpu --format=csv,noheader}°C
Disk: ${fs_used /} / ${fs_size /} ${alignr}Usage: ${fs_used_perc /}%
Network: ${downspeed wlp2s0} ↓ ${upspeed wlp2s0} ↑
]]