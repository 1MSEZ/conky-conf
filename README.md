# conky-conf
-- vim: ts=4 sw=4 noet ai cindent syntax=lua

conky.config = {
    own_window_hints = 'undecorated,below,sticky,skip_taskbar,skip_pager',
    own_window_transparent = false,
    own_window_argb_visual = true,
    own_window_argb_value = 60,
    own_window_colour = yellow,
    alignment = 'top_right',
    background = true,
    border_width = 2,
    cpu_avg_samples = 2,
	default_color = 'lightyellow',
    default_outline_color = 'lightyellow',
    default_shade_color = 'lightyellow',
    draw_borders = true,
    draw_graph_borders = true,
    draw_outline = false,
    draw_shades = false,
    use_xft = true,
    font = 'DejaVu Sans Mono:size=11',
    gap_x = 20,
    gap_y = 60,
    minimum_height = 5,
	minimum_width = 5,
    net_avg_samples = 2,
    no_buffers = true,
    out_to_console = false,
    out_to_stderr = false,
    extra_newline = false,
    own_window = true,
    own_window_class = 'Conky',
    own_window_type = 'desktop',
    stippled_borders = 0,
    update_interval = 1.0,
    uppercase = false,
    use_spacer = 'none',
    show_graph_scale = true,
    show_graph_range = true
}

conky.text = [[
${color lightblue}blue x GuardiaN Conky
$hr
${color green}System Uptime:$color $uptime
${color green}CPU Frequency (in MHz):$color $freq
${color green}CPU Frequency (in GHz):$color $freq_g
${color green}RAM Usage:$color $mem/$memmax - $memperc% ${membar 4}
${color green}Swap Usage:$color $swap/$swapmax - $swapperc% ${swapbar 4}
${color green}CPU Usage:$color $cpu% ${cpubar 4}
${color green}Processes:$color $processes  ${color grey}Running:$color $running_processes
$hr
${color green}Elemetary File Systems:
 / $color${fs_used /}/${fs_size /} ${fs_bar 6 /}
${color green}Network Status:
${color lightyellow}Up:$color ${upspeed enp114s0} ${color lightyellow} - Down:$color ${downspeed enp114s0}
$hr
${color green} Name               PID   CPU%   MEM%
${color lightyellow} ${top name 1} ${top pid 1} ${top cpu 1} ${top mem 1}
${color lightyellow} ${top name 2} ${top pid 2} ${top cpu 2} ${top mem 2}
${color lightyellow} ${top name 3} ${top pid 3} ${top cpu 3} ${top mem 3}
${color lightyellow} ${top name 4} ${top pid 4} ${top cpu 4} ${top mem 4}
]]
