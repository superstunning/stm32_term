# stm32_term
terminal for stm32, you can communication with stm32 app by using tool : Tera Term etc.
if you are debuging an application, you can using this term to display log informations or send commands to stm32 for checking or testing some functions.
you can use terminal tool, for example : tera term or other terminal tools.
tera term can be downloaded from : http://ttssh2.osdn.jp/

you can set log out level (using tera term).
>log level=[debug/info/warning/error]

you can log out some messages to display on tera term by using stm32 function : 

>void log_debug(const char* tag, const char* msg)

>void log_info(const char* tag, const char* msg)

>void log_warning(const char* tag, const char* msg)

>void log_error(const char* tag, const char* msg)


you can set log out level by using stm32 function :

>void log_set_level(uint8_t level)

priority level :  error > warning > info > debug
  
for example, level is warning, the messages can be displayed are error/warning, info and debug can not be displayed.

we use uart1 for terminal function.
you also can change source tu use uart2/3/4/5 for terminal function.
  
  
