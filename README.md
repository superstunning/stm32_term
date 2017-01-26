# stm32_term
terminal for stm32f103/gd32f103, you can do communication with stm32 app by using tool : Tera Term etc.
if you are debuging an application, you can using this term to display log informations or send commands to stm32 for checking or testing some functions.
you can use terminal tool, for example : tera term or other terminal tools.
tera term can be downloaded from : http://ttssh2.osdn.jp/


# functions
you can log out some messages to display on tera term by using stm32 function : 

  >void log_debug(const char* tag, const char* msg)

  >void log_info(const char* tag, const char* msg)

  >void log_warning(const char* tag, const char* msg)

  >void log_error(const char* tag, const char* msg)

you can set log out level by using stm32 function :

  >void log_set_level(uint8_t level)

# log priority level
priority level :  error > warning > info > debug

you can set log out level (using tera term).
  >log level=[debug/info/warning/error]

for example, level is warning, the messages can be displayed are error/warning, info and debug can not be displayed.

# GD32F103 series
if you want to use gd32 series mcu, you must add a preprocessor symbol __GD32F10X__.

# development tools
  keil for arm v5.16.0.0

# contact me
you can send e-mail to me : zhu_yanjun@superstunning.com


  
