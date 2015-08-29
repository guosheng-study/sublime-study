# sublime-study

###官网
http://www.sublimetext.com/  
http://www.sublimetext.com/2  
http://www.sublimetext.com/3  

###注册码：

----- BEGIN LICENSE ------ 
Alexander 
Single User License 
EA7E-814345 
51F47F09 4EAB1285 7827EFF0 8B1207DC 
A76A6EA3 E1A1CA7A DC1F2703 14,897,784 
8EDC1C82 3F2A58B9 1C0C8B24 67686432 
281245B3 6233DE5C ADC5C2F9 61FB8A04 
171B63EF 86BA423F 6AC884FD 3273A7AA 
5F50A6DB CE7859AE D62D2B37 AEEDD8C2 
078A8A20 70EEA791 84F48C1E 8ABA7DEB 
0B3907C0 C9A3523B 0091A045 6F67AED8 
------ END LICENSE ------

###安装控制台
The simplest method of installation is through the Sublime Text console. The console is accessed via the ctrl+` shortcut or the View > Show Console menu. Once open, paste the appropriate Python code for your version of Sublime Text into the console.

**Sublime Text 3**    
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)


**Sublime Text 2**     
import urllib2,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')

###使用Package Control组件安装插件    
按下Ctrl+Shift+P调出命令面板，输入install， 调出 Install Package 选项并回车，然后在列表中选中要安装的插件。





###相关网址
