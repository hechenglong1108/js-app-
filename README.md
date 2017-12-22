# js调app的方法
--
/**
* JS脚本调用APP原生口子（函数）的书写方式
* 这里要考虑兼容IOS/Andriod 两种机型 所以会用到try catch机制
* functionName:是口子（函数）名称 注意替换
*/

try {
    //IOS
    
    window.webkit.messageHandlers.NativeMethod.functionName();
    
}catch(e){

	try{
	
	    //Android
	    
	    window.control.functionName();
	    
	}catch(eg)
	
	{
	
		alert("无法跳转XX函数");
		
	}
	
}
