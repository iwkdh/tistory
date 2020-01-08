	//오늘 하루 안보기, 닫기
	//쿠키설정	
	function setCookie( name, value, expiredays )
	{
	var todayDate = new Date();
	todayDate.setDate( todayDate.getDate() + expiredays );
	document.cookie = name + '=' + escape( value ) + '; path=/; expires=' + todayDate.toGMTString() + ';'
	}
	//쿠키 불러오기
	function getCookie(name) 
	{ 
			var obj = name + "="; 
			var x = 0; 
			while ( x <= document.cookie.length ) 
			{ 
					var y = (x+obj.length); 
					if ( document.cookie.substring( x, y ) == obj ) 
					{ 
							if ((endOfCookie=document.cookie.indexOf( ";", y )) == -1 ) 
									endOfCookie = document.cookie.length;
							return unescape( document.cookie.substring( y, endOfCookie ) ); 
					} 
					x = document.cookie.indexOf( " ", x ) + 1; 
					if ( x == 0 ) 
							break; 
			} 
			return ""; 
	}
	//닫기 버튼 클릭시
	function closewin(key)
	{
			if($("#today").prop("checked")) {
					setCookie('one'+key, 'Y' , 1 );
			}
			$("#one"+key+"").hide();
	}

	$(function(){	
		if(getCookie("one1") !="Y"){
			$("#one1").show();
		}
	});
