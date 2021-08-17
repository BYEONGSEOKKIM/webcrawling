```python
import requests
```


```python
req = requests.get("http://movie.naver.com")
```


```python
text = req.text
```


```python
print(text)
```

    
    
    
    
    
    
    
    
    <!DOCTYPE html>
    <html lang="ko">
    <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="imagetoolbar" content="no">
    <meta property="og:title" content="네이버 영화"/>
    <meta property="og:description" content="영화에 대한 모든 것"/>
    <meta property="og:image" content="https://ssl.pstatic.net/static/m/movie/icons/OG_270_270.png"/>
    <meta property="og:type" content="article"/>
    <meta property="og:url" content="https://movie.naver.com"/>
    <title>네이버 영화</title>
    
    
    
    	
    	
    	
    	
    		<link rel="shortcut icon" href="https://ssl.pstatic.net/static/m/movie/icons/naver_movie_favicon.ico" type="image/x-icon">
    			
    
    
    
    <link rel="stylesheet" type="text/css" href="/css/deploy/movie.all.css?20210728101151" />
    
    <script type="text/javascript" src="/js/deploy/movie.home.js?20210728101151"></script>
    </head>
    
    <body >
    <div id="wrap" class="basic">
    
    	<!-- GNB -->
    	
    
    
    
    <script type="text/javascript">
    function delayed_submit(object) {
    	if (navigator.userAgent.indexOf('MSIE') == -1) {
    		var b = c = new Date();
          	while ((b.getTime() - c.getTime()) < 100) {
    			b = new Date();
          	}
    	} 
    }
    </script>
    
    <script type="text/javascript">
    	var gnb_service = "movie";
    	var gnb_logout = "https://movie.naver.com/index.naver";
    	var gnb_template = "gnb_utf8";
    	var gnb_brightness=3;
    	var gnb_response = true;
    	
    	jindo.$Fn(function(){
    		getGNB();
    	}).attach(window, "load");
    	
    	jindo.$Fn(function(oEvent){ var welSource = jindo.$Element(oEvent.element);
    			if (!welSource.isChildOf(jindo.$Element("gnb"))) {
    				gnbAllLayerClose();
    			}
    	}).attach(document, 'click');
    </script>
     <!-- skip navigation -->
    <div id="u_skip">
             <a href="#header" onclick="document.getElementById('header').tabIndex=-1;document.getElementById('header').focus();return false;"><span>메인 메뉴로 바로가기</span></a>
             <a href="#content" id="gnb_goContent" onclick="document.getElementById('content').tabIndex=-1;document.getElementById('content').focus();return false;"><span>본문으로 바로가기</span></a>
    </div>
    <!-- //skip navigation -->
    <div class="gnb_container">
    	<div class="gnb_content">
    		<div class="gnb_box">
    			<div class="gnb_wrap">
    				<div id="gnb">
    				    <script type="text/javascript" charset="utf-8" src="https://ssl.pstatic.net/static.gn/templates/gnb_utf8.nhn"></script>
    				</div>
    			</div>
    			<!-- 검색창 -->
    			<form id="jSearchForm" action="/movie/search/result.naver" method="get" style="margin:0;display:none;">
    				<input type="text" name="query" maxlength="100" title="영화검색" />
    				<input type="hidden" name="section" value="all"/>
    				<input type="hidden" name="ie" value="utf8"/>
    			</form>
    			<fieldset id="jSearchArea" class="srch_area">
    				<legend><span class="blind">영화검색 영역</span></legend>
    				<div class="srch_field_on _view">
    					<span class="ipt_srch">
    						<label for="ipt_tx_srch" id="search_placeholder">영화검색</label>
    						<input type="text" id="ipt_tx_srch" class="ipt_tx_srch" name="query" maxlength="100" accesskey="s" style="ime-mode:active;" autocomplete="off" />
    						<span class="align"></span>
    						<span class="auto_tx"><a href="#" title="자동완성 펼치기"><img src="https://ssl.pstatic.net/static/movie/2012/06/srch_arrow_down.gif" width="7" height="4" title="자동완성 펼치기" alt="자동완성 펼치기" /></a></span>
    					</span>
    					<button type="submit" title="검색" class="btn_srch" onClick="clickcr(this,'GNB.search','','',event); delayed_submit(this);"><span class="blind">검색</span></button>
    					 <!-- 자동 완성 영역임 #autocomplate_template-->
    				</div>
    			</fieldset>
    			<!-- //검색창 -->
    		</div>
    	</div>
    </div>
    
    	<!-- //GNB -->
    
    	<!-- header -->
    	
    
    
    
    
    
    	<div id="header">
    		<a href="#content" title="본문으로 이동" class="blind">본문 바로가기</a>
    		<h1 class="svc_name">
    			<a href="http://www.naver.com/" title="naver로 바로가기" class="ci_logo" id="lnb_gonaver"><img src="https://ssl.pstatic.net/static/movie/2013/07/logo_ci.png" width="62" height="13" alt="NAVER" /></a><!-- N=a:LNB.naver -->
    			<a href="/" title="영화서비스홈으로 바로가기" class="svc_logo"><img src="https://ssl.pstatic.net/static/movie/2012/06/logo_svc.png" width="34" height="19" alt="영화" /></a><!-- N=a:LNB.movie -->
    		</h1>
    		<div id="scrollbar" class="scrollbar scrollbar-noscript">
    			<div class="scrollbar-box">
    				<div class="scrollbar-content">
                        <div class="in_scroll">
                            <ul class="navi">
                            <li>
                                <a href="/" title="영화홈" class="menu01_on"><strong>영화홈</strong></a><!-- N=a:LNB.home -->
                            </li>
                            <li>
                                <a href="/movie/running/current.naver" title="상영작·예정작" class="menu02"><strong>상영작·예정작</strong></a><!-- N=a:LNB.movies -->
                                <ul class="navi_sub" id="navi_movie" style="display:none">
                                <li><a href="/movie/running/current.naver" title="현재 상영영화" class="sub2_1"><em>현재 상영영화</em></a><!-- N=a:LNB.now --></li>
                                <li><a href="/movie/running/premovie.naver" title="개봉 예정영화" class="sub2_2"><em>개봉 예정영화</em></a><!-- N=a:LNB.soon --></li>
                                
                                <li><a href="/movie/running/movieclip.naver" title="예고편" class="sub2_4"><em>예고편</em></a><!-- N=a:LNB.tailer --></li>
                                </ul>
                            </li>
                            <li>
                                <a href="/movie/sdb/rank/rmovie.naver" title="영화랭킹" class="menu03"><strong>영화랭킹</strong></a><!-- N=a:LNB.db -->
                            </li>
                            <li>
                                <a href="/movie/bi/mi/reserve.naver" title="예매" class="menu05"><strong>예매</strong></a><!-- N=a:LNB.ticket -->
                            </li>
    
                            <li>
    							<a href="/movie/point/af/list.naver" title="평점&middot리뷰" class="menu07"><strong>평점&middot리뷰</strong></a><!-- N=a:LNB.comm -->
                            </li>
                            <li>
                                <a href="https://serieson.naver.com/movie/home.nhn" title="다운로드" class="menu08" target="_blank"><strong>다운로드</strong></a><!-- N=a:LNB.download -->
                            </li>
    						<li class="nav_indi">
    						        <a href="http://tv.naver.com/indiecinema" title="인디극장 UP" target="_blank"><strong>인디극장 UP</strong></a><!-- N=a:LNB.indie -->
    						</li>                        
                            </ul>
                            
                        </div>
    				</div>
    			</div>
    			<div class="scrollbar-v">
    				<div class="scrollbar-button-up"></div>
    				<div class="scrollbar-track">
    					<div class="scrollbar-thumb"></div>
    				</div>
    				<div class="scrollbar-button-down"></div>
    			</div>
    		</div>
    	</div>
    	
    	<script type="text/javascript">
    	if ("영화홈" == "상영작·예정작"
    			|| "영화홈" == "현재 상영영화"
    			|| "영화홈" == "개봉 예정영화"
    			|| "영화홈" == "TV 방영영화"
    			|| "영화홈" == "예고편") {
    		jindo.$Element("navi_movie").show();
    	}
    	</script>
    	<!-- //header -->
    	
    	<!-- container -->
    	<div id="container">
    			<!-- content -->
    <div id="content">
    
    	
    	<div class="article hh">
    		<h2 class="blind">영화홈</h2>
    		<!-- 무비차트 -->
    		<div class="mv_main" onmouseover="oTimer.abort();" onmouseout="movieChart.restartTimer();">
    			<div class="running_tab">
    				<ul>
    					<li id="RESERVE_tab" class="item on"><a href="#none" onclick="movieChart.fullSettingMovieChart(0);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" class="flickingTab"><em>예매순</em></a><!-- N=a:run.ticket --></li>
    					<li id="CURRENT_tab" class="item"><a href="#none" onclick="movieChart.fullSettingMovieChart(1);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" class="flickingTab"><em>현재상영작</em></a><!-- N=a:run.now --></li>
    					<li id="COMMING_tab" class="item"><a href="#none" onclick="movieChart.fullSettingMovieChart(2);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" class="flickingTab"><em>개봉예정작</em></a><!-- N=a:run.coming --></li>
    					<li id="POINT_tab" class="item"><a href="#none" onclick="movieChart.fullSettingMovieChart(3);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" class="flickingTab"><em>평점순</em></a><!-- N=a:run.bystar --></li>
    					<li id="BOXOFFICE_tab" class="item"><a href="#none" onclick="movieChart.fullSettingMovieChart(4);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" class="flickingTab"><em>박스오피스</em></a><!-- N=a:run.box --></li>
    					<li id="DOWNLOAD_tab" class="item"><a href="#none" onclick="movieChart.fullSettingMovieChart(5);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" class="flickingTab"><em>다운로드순</em></a><!-- N=a:run.down --></li>
    				</ul>
    			</div>
    			<!-- flick area -->
    			<div id="mflick" class="flick_view_area flick-view">
    				<div class="flick-container" style="left: 0px; ">
    					<strong id="pannel0" class="blind"></strong>
    					<ul id="flick0" class="flick-ct home_list page0 flick-panel" style="display:none;"></ul>
    					<strong id="pannel1" class="blind"></strong>
    					<ul id="flick1" class="flick-ct home_list page1 flick-panel"></ul>
    					<strong id="pannel2" class="blind"></strong>
    					<ul id="flick2" class="flick-ct home_list page2 flick-panel" style="display:none;"></ul>
    				</div>
    			</div>
    			<!-- //flick area -->
    			<!-- [D] 다운로드순 클릭시 p에 클래스 dwn 추가 다른 버튼 클릭시 클래스 삭제 <p class="all_view_go dwn"> -->
    			<p class="all_view_go" id="_all_view_go"><a id="movieChartAllView" href="/movie/running/premovie.naver" onclick="clickcr(this, 'run.all', '', '', event);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" title="전체보기">전체보기</a></p>
    			<div class="flick_nav">
    				<a href="#" id="flick_prev" class="btn_prev" onclick="clickcr(this, 'run.pre', '', '', event);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" title="이전"><em>이전</em></a><!-- N=a:run.pre -->
    			</div>
    			<div class="flick_nav">
    				<a href="#" id="flick_next" class="btn_next" onclick="clickcr(this, 'run.next', '', '', event);" onfocus="oTimer.abort();" onblur="movieChart.restartTimer();" title="다음"><em>다음</em></a><!-- N=a:run.next -->
    			</div>
    		</div>
    		<!-- //무비차트  -->
    		<div class="section_group" id="homeReview">
    			<div class="obj_section">
    				<div class="main_review">
    					
    					<div class="title_area">
    						<h4 class="hh_review"><strong class="blind">개봉영화 평점</strong></h4>
    					</div>
    					<div class="hh_review_area">
    						<div id="movieReview" class="hh_review_ct">
    							<ul class="lst_con first" data-index=0 style="display:block">
    							<!-- [D] 선택된 경우 li에 class="on" 추가 -->
    							
    							<li id="review1" data-index=0 class="_select_title">
    								<a href="/movie/bi/mi/basic.naver?code=191597" class="thmb" onclick="clickcr(this, 'tvw.img', '191597', '1', event);"><img src="https://movie-phinf.pstatic.net/20210622_174/1624324910624JhEq2_JPEG/movie_image.jpg?type=f64_91" width="64" height="91" alt="보스 베이비 2" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img64x91.png'"></a>
    								<div class="detail">
    									<a href="/movie/bi/mi/basic.naver?code=191597" onclick="clickcr(this, 'tvw.title', '191597', '1', event);" data-index=0 class="_select_title_anchor"><strong>보스 베이비 2</strong>
    										<div class="star_score">
    											
    											
    											
    												
    												
    													
    													
    													
    													<span class="st_off"><span class="st_on" style="width:91.4%">평점 - 총 10점 중</span></span>
    													<span class="score">
    													<span class="char sc_num9"><em>9</em></span><span class="char sc_dot"><em>.</em></span><span class="char sc_num1"><em>1</em></span><span class="char sc_num4"><em>4</em></span>
    												
    											
    											</span>
    										</div>
    									</a>
    									<ul class="info">
    										
    											
    												<li><a href="/movie/bi/mi/point.naver?code=191597&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17609059', '1', event);"><span class="tit">가볍게 보러갔다가 감동까지 느끼고 옵니다올해 봤던 애니메이션 중에 제일 재밌게 봤네요</span></a></li>
    											
    										
    											
    												<li><a href="/movie/bi/mi/point.naver?code=191597&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17608937', '2', event);"><span class="tit">귀여워서 심장 아픔ㅠㅠ 세상에 이런 보스라면 매일 출근하궤쒀!!</span></a></li>
    											
    										
    											
    												<li class="last"><a href="/movie/bi/mi/point.naver?code=191597&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17609015', '3', event);"><span class="tit">귀여운 아가보스가 두명이나 나오는데 비주얼적으로 안볼수가 없지요!!^^ 1편도 재미있게 봤었는데, 2편은 더더 경쾌하고 액션 넘쳐서 즐겁게 볼수 있었어요. 이 사랑스러운 영화 추천합니다!!</span></a></li>
    											
    										
    									</ul>
    								</div>
    							</li>
    							
    							<li id="review2" data-index=1 class="_select_title">
    								<a href="/movie/bi/mi/basic.naver?code=196049" class="thmb" onclick="clickcr(this, 'tvw.img', '196049', '2', event);"><img src="https://movie-phinf.pstatic.net/20210805_35/1628142193088hCOyc_JPEG/movie_image.jpg?type=f64_91" width="64" height="91" alt="극장판 도라에몽: 진구의 신공룡" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img64x91.png'"></a>
    								<div class="detail">
    									<a href="/movie/bi/mi/basic.naver?code=196049" onclick="clickcr(this, 'tvw.title', '196049', '2', event);" data-index=1 class="_select_title_anchor"><strong>극장판 도라에몽: 진구의 신공룡</strong>
    										<div class="star_score">
    											
    											
    											
    												
    												
    													
    													
    													
    													<span class="st_off"><span class="st_on" style="width:92.5%">평점 - 총 10점 중</span></span>
    													<span class="score">
    													<span class="char sc_num9"><em>9</em></span><span class="char sc_dot"><em>.</em></span><span class="char sc_num2"><em>2</em></span><span class="char sc_num5"><em>5</em></span>
    												
    											
    											</span>
    										</div>
    									</a>
    									<ul class="info">
    										
    											
    												<li><a href="/movie/bi/mi/point.naver?code=196049&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17634016', '1', event);"><span class="tit">머랄까 그냥 행복해지네요</span></a></li>
    											
    										
    											
    												<li><a href="/movie/bi/mi/point.naver?code=196049&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17637842', '2', event);"><span class="tit">저학년 아들 때문에 피곤한 몸으로 도라에몽 보러 갔습니다. 전 도라에몽 본적도 없고 관심도 없어서 억지로 끌려간건데 마지막 순간 울컥하는 제 자신을 발견했습니다. 40대입니다. 며칠전 모가디슈 재미있게 봤었는데 도라에몽이 더 대작이네요. 아이들 영화라고 무시했던 저를 반성합니다.</span></a></li>
    											
    										
    											
    												<li class="last"><a href="/movie/bi/mi/point.naver?code=196049&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17639113', '3', event);"><span class="tit">팬들도 아이들도 따라 보러온 어른들도 모두 감동시키는 영화. 50주년에 걸맞는 대작이라고 생각합니다. 옛 극장판을 상기시키는 오마주와 연출에 감동했습니다. 감독과 각본이 같은 &#34;진구의 보물섬&#34;이라는 영화도 있으니 이번 영화에 만족하신분은 보물섬을 꼭 보시기 바랍니다! </span></a></li>
    											
    										
    									</ul>
    								</div>
    							</li>
    							
    							<li id="review3" data-index=2 class="_select_title">
    								<a href="/movie/bi/mi/basic.naver?code=188472" class="thmb" onclick="clickcr(this, 'tvw.img', '188472', '3', event);"><img src="https://movie-phinf.pstatic.net/20210726_114/1627265960693kkM0B_JPEG/movie_image.jpg?type=f64_91" width="64" height="91" alt="싱크홀" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img64x91.png'"></a>
    								<div class="detail">
    									<a href="/movie/bi/mi/basic.naver?code=188472" onclick="clickcr(this, 'tvw.title', '188472', '3', event);" data-index=2 class="_select_title_anchor"><strong>싱크홀</strong>
    										<div class="star_score">
    											
    											
    											
    												
    												
    													
    													
    													
    													<span class="st_off"><span class="st_on" style="width:68.6%">평점 - 총 10점 중</span></span>
    													<span class="score">
    													<span class="char sc_num6"><em>6</em></span><span class="char sc_dot"><em>.</em></span><span class="char sc_num8"><em>8</em></span><span class="char sc_num6"><em>6</em></span>
    												
    											
    											</span>
    										</div>
    									</a>
    									<ul class="info">
    										
    											
    												<li><a href="/movie/bi/mi/point.naver?code=188472&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17646383', '1', event);"><span class="tit">기대보다 별로였어요..</span></a></li>
    											
    										
    											
    												<li><a href="/movie/bi/mi/point.naver?code=188472&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17645992', '2', event);"><span class="tit">휴~ 90년대 개그와 cg…긴장감 전혀 없는 재난영화??</span></a></li>
    											
    										
    											
    												<li class="last"><a href="/movie/bi/mi/point.naver?code=188472&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17647764', '3', event);"><span class="tit">댓글 알바가 판을 치는군요 보면 압니다..</span></a></li>
    											
    										
    									</ul>
    								</div>
    							</li>
    							
    							<li id="review4" data-index=3 class="_select_title">
    								<a href="/movie/bi/mi/basic.naver?code=184318" class="thmb" onclick="clickcr(this, 'tvw.img', '184318', '4', event);"><img src="https://movie-phinf.pstatic.net/20210617_272/1623906098516QjpeS_JPEG/movie_image.jpg?type=f64_91" width="64" height="91" alt="블랙 위도우" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img64x91.png'"></a>
    								<div class="detail">
    									<a href="/movie/bi/mi/basic.naver?code=184318" onclick="clickcr(this, 'tvw.title', '184318', '4', event);" data-index=3 class="_select_title_anchor"><strong>블랙 위도우</strong>
    										<div class="star_score">
    											
    											
    											
    												
    												
    													
    													
    													
    													<span class="st_off"><span class="st_on" style="width:85.0%">평점 - 총 10점 중</span></span>
    													<span class="score">
    													<span class="char sc_num8"><em>8</em></span><span class="char sc_dot"><em>.</em></span><span class="char sc_num5"><em>5</em></span><span class="char sc_num0"><em>0</em></span>
    												
    											
    											</span>
    										</div>
    									</a>
    									<ul class="info">
    										
    											
    												<li><a href="/movie/bi/mi/point.naver?code=184318&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17584312', '1', event);"><span class="tit">스칼렛 요한슨  고생했어요 </span></a></li>
    											
    										
    											
    												<li><a href="/movie/bi/mi/point.naver?code=184318&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17584090', '2', event);"><span class="tit">항상 마블 영화에서 위도우 씬이 편집 삭제됐었는데 이 기회에 블랙위도우 서사를 마무리할 수 있어서 좋았음 액션도 쾌속있고 굿</span></a></li>
    											
    										
    											
    												<li class="last"><a href="/movie/bi/mi/point.naver?code=184318&onlyActualPointYn=Y#pointAfterListIframe" onclick="clickcr(this, 'tvw.list', '17584191', '3', event);"><span class="tit">은근히 다크한 분위기인데 그만큼 진지한 스토리라서 몰입해서 봄. 어린시절 훈련내용은 없어서 아쉬웠지만, 바디액션이 짱짱해서 재밌음. 쿠키 하나 있으니까 꼭 보세요. </span></a></li>
    											
    										
    									</ul>
    								</div>
    							</li>
    							
    							</ul>
    						</div>
    					</div>
    				</div>
    				<div class="main_spot" id="homeSpotlight">
    					
    					<div class="section">
    						<div class="title_area">
    							<h4 class="hh_spotlight">
    								<strong class="blind">스포트라이트</strong>
    							</h4>
    						</div>
    						<div class="hh_spot_area">
    							<a href="https://serieson.naver.com/event/details.nhn?eventNo=13517&productType=MOVIE">
    								
    								
    									
    								
    								<img src="https://movie-phinf.pstatic.net/20210804_51/16280511715624ume3_JPEG/__210x190.jpg" width="210" height="196" title="스포트라이트 배너" alt="밀리언 달러 트러블 오픈 프로모션" border="0">
    							</a>
    						</div>
    					</div>
    					
    				</div>
    			</div>
    
    			
    			<div class="obj_section" id="homeTrailer">
    				<div class="main_prv">
    					<div class="title_area">
    						<h4 class="hh_preview"><strong class="blind">예고편</strong></h4>
    					</div>
    					<ul class="video_thumb">
    					
    					<li>
    						<a href="/movie/bi/mi/mediaView.naver?code=201727&mid=50172#tab" title="메인 예고편" class="video_obj">
    							<span class="mask">동영상</span>
    							
    							<span class="video_ico first"><span class="blind">최초</span></span>
    							<img src="https://ssl.pstatic.net/imgmovie/multimedia/MOVIECLIP/TRAILER/50172_20210813014332.jpg" width="164" height="114" alt="메인 예고편" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img164x114.png'">
    						</a><!-- N=a:cms.img,r:1,i:50172 -->
    						<p class="tx_video ico"><a href="/movie/bi/mi/mediaView.naver?code=201727&mid=50172#tab" title="대테러부대: 팀 울프">대테러부대: 팀 울프</a><!-- N=a:cms.title,r:1,i:50172 --></p>
    						<p class="tx_brief"><a href="/movie/bi/mi/mediaView.naver?code=201727&mid=50172#tab" title="메인 예고편">메인 예고편</a><!-- N=a:cms.desc,r:1,i:50172 --></p>
    					</li>
    					
    					<li>
    						<a href="/movie/bi/mi/mediaView.naver?code=178805&mid=50173#tab" title="메인 예고편" class="video_obj">
    							<span class="mask">동영상</span>
    							
    							<span class="video_ico first"><span class="blind">최초</span></span>
    							<img src="https://ssl.pstatic.net/imgmovie/multimedia/MOVIECLIP/TRAILER/50173_20210813014414.jpg" width="164" height="114" alt="메인 예고편" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img164x114.png'">
    						</a><!-- N=a:cms.img,r:2,i:50173 -->
    						<p class="tx_video ico"><a href="/movie/bi/mi/mediaView.naver?code=178805&mid=50173#tab" title="마더스 인스팅트">마더스 인스팅트</a><!-- N=a:cms.title,r:2,i:50173 --></p>
    						<p class="tx_brief"><a href="/movie/bi/mi/mediaView.naver?code=178805&mid=50173#tab" title="메인 예고편">메인 예고편</a><!-- N=a:cms.desc,r:2,i:50173 --></p>
    					</li>
    					
    					<li>
    						<a href="/movie/bi/mi/mediaView.naver?code=191907&mid=50179#tab" title="메인 예고편" class="video_obj">
    							<span class="mask">동영상</span>
    							
    							<span class="video_ico first"><span class="blind">최초</span></span>
    							<img src="https://ssl.pstatic.net/imgmovie/multimedia/MOVIECLIP/TRAILER/50179_20210813051734.jpg" width="164" height="114" alt="메인 예고편" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img164x114.png'">
    						</a><!-- N=a:cms.img,r:3,i:50179 -->
    						<p class="tx_video ico"><a href="/movie/bi/mi/mediaView.naver?code=191907&mid=50179#tab" title="어시스턴트">어시스턴트</a><!-- N=a:cms.title,r:3,i:50179 --></p>
    						<p class="tx_brief"><a href="/movie/bi/mi/mediaView.naver?code=191907&mid=50179#tab" title="메인 예고편">메인 예고편</a><!-- N=a:cms.desc,r:3,i:50179 --></p>
    					</li>
    					
    					<li>
    						<a href="/movie/bi/mi/mediaView.naver?code=196578&mid=50174#tab" title="티저 예고편" class="video_obj">
    							<span class="mask">동영상</span>
    							
    							<span class="video_ico first"><span class="blind">최초</span></span>
    							<img src="https://ssl.pstatic.net/imgmovie/multimedia/MOVIECLIP/TRAILER/50174_20210813014503.jpg" width="164" height="114" alt="티저 예고편" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img164x114.png'">
    						</a><!-- N=a:cms.img,r:4,i:50174 -->
    						<p class="tx_video ico"><a href="/movie/bi/mi/mediaView.naver?code=196578&mid=50174#tab" title="첫눈이 사라졌다">첫눈이 사라졌다</a><!-- N=a:cms.title,r:4,i:50174 --></p>
    						<p class="tx_brief"><a href="/movie/bi/mi/mediaView.naver?code=196578&mid=50174#tab" title="티저 예고편">티저 예고편</a><!-- N=a:cms.desc,r:4,i:50174 --></p>
    					</li>
    					
    					</ul>
    					<a href="/movie/running/movieclip.naver" class="link_more">더보기<span class="ico_more"></span></a><!-- N=a:cms.more -->
    				</div>
    			</div>
    		</div>
    		
    
    		
    		<div class="section_group" id="homePhoto">
    			<div class="obj_section">
    				<div class="main_photo">
    					<div class="title_area">
    						<h4 class="hh_photo"><strong class="blind">포토</strong></h4>
    					</div>
    					<ul>
    					
    					<li class="">
    						<p class="thmb">
    							<a href="/movie/bi/mi/photoView.naver?code=204768&imageNid=6735773#tab">
    								<img src="https://movie-phinf.pstatic.net/20210719_291/16266695142998cakT_JPEG/movie_image.jpg?type=n108_108_2" width="108" height="108" alt="새로운 모험" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img108x108.png'">
    								
    								
    							</a><!-- N=a:pho.img,r:1,i:6735773 -->
    						</p>
    						<a href="/movie/bi/mi/photoView.naver?code=204768&imageNid=6735773#tab"><strong class="tit">그린 나이트</strong></a><!-- N=a:pho.list,r:1,i:6735773 -->
    						<p class="tx_brief"><a href="/movie/bi/mi/photoView.naver?code=204768&imageNid=6735773#tab">새로운 모험</a><!-- N=a:pho.tlist,r:1,i:6735773 --></p>
    					</li>
    					
    					<li class="">
    						<p class="thmb">
    							<a href="/movie/bi/mi/photoView.naver?code=196049&imageNid=6734744#tab">
    								<img src="https://movie-phinf.pstatic.net/20210709_300/1625797463053UCTeM_JPEG/movie_image.jpg?type=n108_108_2" width="108" height="108" alt="수수께끼의 섬" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img108x108.png'">
    								
    								
    							</a><!-- N=a:pho.img,r:2,i:6734744 -->
    						</p>
    						<a href="/movie/bi/mi/photoView.naver?code=196049&imageNid=6734744#tab"><strong class="tit">극장판 도라에몽: 진구의 신공룡</strong></a><!-- N=a:pho.list,r:2,i:6734744 -->
    						<p class="tx_brief"><a href="/movie/bi/mi/photoView.naver?code=196049&imageNid=6734744#tab">수수께끼의 섬</a><!-- N=a:pho.tlist,r:2,i:6734744 --></p>
    					</li>
    					
    					<li class="">
    						<p class="thmb">
    							<a href="/movie/bi/mi/photoView.naver?code=167569&imageNid=6734968#tab">
    								<img src="https://movie-phinf.pstatic.net/20210712_221/16260668855712BSKY_JPEG/movie_image.jpg?type=n108_108_2" width="108" height="108" alt="세상을 구하다" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img108x108.png'">
    								
    								
    							</a><!-- N=a:pho.img,r:3,i:6734968 -->
    						</p>
    						<a href="/movie/bi/mi/photoView.naver?code=167569&imageNid=6734968#tab"><strong class="tit">더 수어사이드 스쿼드</strong></a><!-- N=a:pho.list,r:3,i:6734968 -->
    						<p class="tx_brief"><a href="/movie/bi/mi/photoView.naver?code=167569&imageNid=6734968#tab">세상을 구하다</a><!-- N=a:pho.tlist,r:3,i:6734968 --></p>
    					</li>
    					
    					<li class="">
    						<p class="thmb">
    							<a href="/movie/bi/mi/photoView.naver?code=114330&imageNid=6738024#tab">
    								<img src="https://movie-phinf.pstatic.net/20210810_161/1628560070238K58wn_JPEG/movie_image.jpg?type=n108_108_2" width="108" height="108" alt="혼란에 빠지다" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img108x108.png'">
    								
    								
    							</a><!-- N=a:pho.img,r:4,i:6738024 -->
    						</p>
    						<a href="/movie/bi/mi/photoView.naver?code=114330&imageNid=6738024#tab"><strong class="tit">바쿠라우</strong></a><!-- N=a:pho.list,r:4,i:6738024 -->
    						<p class="tx_brief"><a href="/movie/bi/mi/photoView.naver?code=114330&imageNid=6738024#tab">혼란에 빠지다</a><!-- N=a:pho.tlist,r:4,i:6738024 --></p>
    					</li>
    					
    					<li class="">
    						<p class="thmb">
    							<a href="/movie/bi/mi/photoView.naver?code=202673&imageNid=6720607#tab">
    								<img src="https://movie-phinf.pstatic.net/20210222_178/1613960200630oV4Rn_JPEG/movie_image.jpg?type=n108_108_2" width="108" height="108" alt="특별한 동거" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img108x108.png'">
    								
    								
    							</a><!-- N=a:pho.img,r:5,i:6720607 -->
    						</p>
    						<a href="/movie/bi/mi/photoView.naver?code=202673&imageNid=6720607#tab"><strong class="tit">아임 유어 맨</strong></a><!-- N=a:pho.list,r:5,i:6720607 -->
    						<p class="tx_brief"><a href="/movie/bi/mi/photoView.naver?code=202673&imageNid=6720607#tab">특별한 동거</a><!-- N=a:pho.tlist,r:5,i:6720607 --></p>
    					</li>
    					
    					<li class="last">
    						<p class="thmb">
    							<a href="/movie/bi/mi/photoView.naver?code=167721&imageNid=6594595#tab">
    								<img src="https://movie-phinf.pstatic.net/20180109_2/15154651832167NTOE_JPEG/movie_image.jpg?type=n108_108_2" width="108" height="108" alt="육체적 욕망" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img108x108.png'">
    								
    								
    							</a><!-- N=a:pho.img,r:6,i:6594595 -->
    						</p>
    						<a href="/movie/bi/mi/photoView.naver?code=167721&imageNid=6594595#tab"><strong class="tit">자마</strong></a><!-- N=a:pho.list,r:6,i:6594595 -->
    						<p class="tx_brief"><a href="/movie/bi/mi/photoView.naver?code=167721&imageNid=6594595#tab">육체적 욕망</a><!-- N=a:pho.tlist,r:6,i:6594595 --></p>
    					</li>
    					
    					</ul>
    				</div>
    			</div>
    			<div class="obj_section">
    				<div class="main_event">
    					<div class="notice">
    						<a href="/movie/other/gonggi.naver" class="notice_more">공지사항 더보기</a><!-- N=a:bnt.more -->
    						<div class="info"><a href="/movie/other/gonggi.naver?docID=10000000000030671746"><em>[안내]</em>&nbsp; 네이버 영화 PC 예매 서비스가 종료됩니다.</a><!-- N=a:bnt.list --></div>
    						<p><span class="page_info">정보</span>본 페이지는 나눔글꼴에 최적화 되어있습니다. <a href="http://hangeul.naver.com/font" target="_blank" class="font_inst">나눔글꼴설치<em class="arr"></em></a><!-- N=a:btm.nanumfont --></p>
    					</div>
    				</div>
    			</div>
    		</div>
    	</div>
    	<!-- [D] 맨위로 버튼 div id="content" 기준 top:342px 이상 -->
    	
    <div class="staticbanner" id="floatingTopAnchor" style="bottom:40px">
        <a href="#u_skip" title="맨위로"><img alt="맨위로" src="https://ssl.pstatic.net/static/movie/2012/08/btn_top.png" width="33" height="35"></a><!-- N=a:btm.top -->
    </div>
    <script type="text/javascript">
    jindo.$Fn(function () {
        var welTopAnchor = jindo.$Element('floatingTopAnchor');
        var welContent = jindo.$Element('content');
        var nTopMargin = 342 + welTopAnchor.height();
        var nMaxY;
        var nMinY = 61;
        var oFloatingLayer = new jindo.FloatingLayer(welTopAnchor).attach({
            beforeMove: function (oEvent) {
                // 상단 limit
                nMaxY = welContent.height() - nTopMargin;
                if (oEvent.nY > nMaxY) {
                    oEvent.nY = nMaxY;
                }
    
                 // 하단 limit
                if (oEvent.nY < nMinY) {
                    oEvent.nY = nMinY;
                }
            }
        });
    }).attach(window, 'load');
    </script>
    	<!-- //맨위로 -->
    
    </div>
    <!-- //content -->
    
    <script type="text/template" id="RESERVE_template">
    {for index:movie in RESERVE}
    	<li class="item{=index +1}" data-id="{=movie.movieCode}" data-detail="{=movie.movieCode}" data-reserve="{=movie.movieCode}" onmouseover="jindo.$Element('reserveTooltip{=index+1}').show();" onmouseout="jindo.$Element('reserveTooltip{=index+1}').hide();">
    		<div class="obj_off tab4">
    			<a href="/movie/bi/mi/basic.naver?code={=movie.movieCode}" onfocus="jindo.$Element('reserveTooltip{=index+1}').show();oTimer.abort();" onblur="jindo.$Element('reserveTooltip{=index+1}').hide();movieChart.restartTimer();"><span class="rank"><em>{=index +1}위</em></span>
    				{if movie.adult}
    					<span class="ico_rating_19">청소년 유해물</span>
    				{elseif movie.lastKoreanGrade != null}
    					{js movieChart.getGradeIcon(=movie.lastKoreanGrade.code)}
    				{/if}
    				<span class="mask"></span>
    				<img src="https://movie-phinf.pstatic.net{=movie.posterImageUrl}?type=f125" alt="{js movieChart.replaceDoubleQuotationForHTML(=movie.movieTitle)}" width="125" height="179" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img125x179.png'">
    				<span class="baseplate r">
    					<span class="spr stic_rate l"><em>예매율</em></span>
    					<strong class="l">{js movieChart.numberFont(=movie.formattedReserveRatio, 'rate')}<span class="char rate_pct"><em>%</em></span></strong>
    				</span>
    			</a><!-- N=a:run.da,r:{=index + 1},i:{=movie.movieCode} -->
    		</div>
    		<div  id="reserveTooltip{=index+1}" class="obj_con" style="display:none">
    			<div class="obj_on{js movieChart.tooltipLengthOver(=movie.movieTitle)} {if (index+1)%5 == 0}rt{/if}">
    				<div class="tooltip">
    					<span class="top"></span>
    					<p class="mv_title">{=movie.movieTitle}</p>
    					<span class="bottom"></span><span class="bottom_r"></span>
    				</div>
    			</div>
    		</div>
    	</li>
    {/for}
    </script>
    
    <script type="text/template" id="CURRENT_template">
    {for index:movie in CURRENT}
    	<li class="item{=index +1}" data-id="{=movie.movieCode}" data-detail="{=movie.movieCode}" data-reserve="{=movie.movieCode}" onmouseover="jindo.$Element('currentTooltip{=index+1}').show();" onmouseout="jindo.$Element('currentTooltip{=index+1}').hide();">
    		<div class="obj_off tab4">
    			<a href="/movie/bi/mi/basic.naver?code={=movie.movieCode}" onfocus="jindo.$Element('currentTooltip{=index+1}').show();oTimer.abort();" onblur="jindo.$Element('currentTooltip{=index+1}').hide();movieChart.restartTimer();">
    				{if movie.adult}
    					<span class="ico_rating_19">청소년 유해물</span>
    				{elseif movie.lastKoreanGrade != null}
    					{js movieChart.getGradeIcon(=movie.lastKoreanGrade.code)}
    				{/if}
    				<span class="mask"></span>
    				<img src="https://movie-phinf.pstatic.net{=movie.posterImageUrl}?type=f125" alt="{js movieChart.replaceDoubleQuotationForHTML(=movie.movieTitle)}" width="125" height="179" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img125x179.png'">
    				<span class="baseplate r">
    					<span class="rank_star l"><span class="star_off"><em>별점 - 총 10점 중</em></span><span class="star_on" style="width:{=movie.point*10}%"><em>{=movie.point} 점</em></span></span>
    					<strong class="l">{js movieChart.numberFont(=movie.point, 'sc')}</strong>
    				</span>
    			</a><!-- N=a:run.da,r:{=index + 1},i:{=movie.movieCode} -->
    		</div>
    		<div id="currentTooltip{=index+1}" class="obj_con" style="display:none">
    			<div class="obj_on{js movieChart.tooltipLengthOver(=movie.movieTitle)} {if (index+1)%5 == 0}rt{/if}">
    				<div class="tooltip">
    					<span class="top"></span>
    					<p class="mv_title">{=movie.movieTitle}</p>
    					<span class="bottom"></span><span class="bottom_r"></span>
    				</div>
    			</div>
    		</div>
    	</li>
    {/for}
    </script>
    
    <script type="text/template" id="COMMING_template">
    {for index:movie in COMMING}
    	<li class="item{=index +1}" data-id="{=movie.movieCode}" data-detail="{=movie.movieCode}" data-reserve="{=movie.movieCode}" onmouseover="jindo.$Element('commingTooltip{=index+1}').show();" onmouseout="jindo.$Element('commingTooltip{=index+1}').hide();">
    		<div class="obj_off tab4">
    			<a href="/movie/bi/mi/basic.naver?code={=movie.movieCode}" onfocus="jindo.$Element('commingTooltip{=index+1}').show();oTimer.abort();" onblur="jindo.$Element('commingTooltip{=index+1}').hide();movieChart.restartTimer();">
    				{if movie.adult}
    					<span class="ico_rating_19">청소년 유해물</span>
    				{elseif movie.lastKoreanGrade != null}
    					{js movieChart.getGradeIcon(=movie.lastKoreanGrade.code)}
    				{/if}
    				<span class="mask"></span>
    				<img src="https://movie-phinf.pstatic.net{=movie.posterImageUrl}?type=f125" alt="{js movieChart.replaceDoubleQuotationForHTML(=movie.movieTitle)}" width="125" height="179" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img125x179.png'">
    				<span class="baseplate r">
    					<strong class="l">{js movieChart.numberFont(=movie.openDate, 'rate')}</strong>{if movie.openDate != ''}<span class="spr stic_open l"><em>개봉</em>{/if}</span>
    				</span>
    			</a><!-- N=a:run.da,r:{=index + 1},i:{=movie.movieCode} -->
    		</div>
    		<div id="commingTooltip{=index+1}" class="obj_con" style="display:none">
    			<div class="obj_on{js movieChart.tooltipLengthOver(=movie.movieTitle)} {if (index+1)%5 == 0}rt{/if}">
    				<div class="tooltip">
    					<span class="top"></span>
    					<p class="mv_title">{=movie.movieTitle}</p>
    					<span class="bottom"></span><span class="bottom_r"></span>
    				</div>
    			</div>
    		</div>
    	</li>
    {/for}
    </script>
    
    <script type="text/template" id="POINT_template">
    {for index:movie in POINT}
    	<li class="item{=index +1}" data-id="{=movie.movieCode}" data-detail="{=movie.movieCode}" data-reserve="{=movie.movieCode}" onmouseover="jindo.$Element('pointTooltip{=index+1}').show();" onmouseout="jindo.$Element('pointTooltip{=index+1}').hide();">
    		<div class="obj_off tab4">
    			<a href="/movie/bi/mi/basic.naver?code={=movie.movieCode}" onfocus="jindo.$Element('pointTooltip{=index+1}').show();oTimer.abort();" onblur="jindo.$Element('pointTooltip{=index+1}').hide();movieChart.restartTimer();"><span class="rank"><em>{=index +1}위</em></span>
    				{if movie.adult}
    					<span class="ico_rating_19">청소년 유해물</span>
    				{elseif movie.lastKoreanGrade != null}
    					{js movieChart.getGradeIcon(=movie.lastKoreanGrade.code)}
    				{/if}
    				<span class="mask"></span>
    				<img src="https://movie-phinf.pstatic.net{=movie.posterImageUrl}?type=f125" alt="{js movieChart.replaceDoubleQuotationForHTML(=movie.movieTitle)}" width="125" height="179" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img125x179.png'">
    				<span class="baseplate r">
    					<span class="rank_star l"><span class="star_off"><em>별점 - 총 10점 중</em></span><span class="star_on" style="width:{=movie.point*10}%"><em>{=movie.point} 점</em></span></span>
    					<strong class="l">{js movieChart.numberFont(=movie.point, 'sc')}</strong>
    				</span>
    			</a><!-- N=a:run.da,r:{=index + 1},i:{=movie.movieCode} -->
    		</div>
    		<div id="pointTooltip{=index+1}" class="obj_con" style="display:none">
    			<div class="obj_on{js movieChart.tooltipLengthOver(=movie.movieTitle)} {if (index+1)%5 == 0}rt{/if}">
    				<div class="tooltip">
    					<span class="top"></span>
    					<p class="mv_title">{=movie.movieTitle}</p>
    					<span class="bottom"></span><span class="bottom_r"></span>
    				</div>
    			</div>
    		</div>
    	</li>
    {/for}
    </script>
    
    <script type="text/template" id="BOXOFFICE_template">
    {for index:movie in BOXOFFICE}
    	<li class="item{=index +1}" data-id="{=movie.movieCode}" data-detail="{=movie.movieCode}" data-reserve="{=movie.movieCode}" onmouseover="jindo.$Element('boxofficeTooltip{=index+1}').show();" onmouseout="jindo.$Element('boxofficeTooltip{=index+1}').hide();">
    		<div class="obj_off tab4">
    			<a href="/movie/bi/mi/basic.naver?code={=movie.movieCode}" onfocus="jindo.$Element('boxofficeTooltip{=index+1}').show();oTimer.abort();" onblur="jindo.$Element('boxofficeTooltip{=index+1}').hide();movieChart.restartTimer();"><span class="rank"><em>{=index +1}위</em></span>
    				{if movie.adult}
    					<span class="ico_rating_19">청소년 유해물</span>
    				{elseif movie.lastKoreanGrade != null}
    					{js movieChart.getGradeIcon(=movie.lastKoreanGrade.code)}
    				{/if}
    				<span class="mask"></span>
    				<img src="https://movie-phinf.pstatic.net{=movie.posterImageUrl}?type=f125" alt="{js movieChart.replaceDoubleQuotationForHTML(=movie.movieTitle)}" width="125" height="179" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img125x179.png'">
    				<span class="baseplate r">
    					<span class="spr stic_box l"><em>주말관객</em></span>
    					<strong class="l">{js movieChart.numberFont(=movie.formattedWeekendAudience, 'cnt')}<span class="char cnt_per"><em>명</em></span></strong>
    				</span>
    			</a><!-- N=a:run.da,r:{=index + 1},i:{=movie.movieCode} -->
    		</div>
    		<div id="boxofficeTooltip{=index+1}" class="obj_con" style="display:none">
    			<div class="obj_on{js movieChart.tooltipLengthOver(=movie.movieTitle)} {if (index+1)%5 == 0}rt{/if}">
    				<div class="tooltip">
    					<span class="top"></span>
    					<p class="mv_title">{=movie.movieTitle}</p>
    					<span class="bottom"></span><span class="bottom_r"></span>
    				</div>
    			<div>
    		</div>
    	</li>
    {/for}
    </script>
    
    <script type="text/template" id="DOWNLOAD_template">
    {if DOWNLOAD ==  ""}
    	<li class="error_area">
    		<div class="error_msg">
    			<p class="blind">
    				죄송합니다. 서비스 점검중입니다. 다운로드 서버와의 통신이 원활하지 않습니다. 잠시 후 다시 시도해주시기 바랍니다.
    			</p>
    		</div>
    	</li>
    {else}
    	{for index:movie in DOWNLOAD}
    		<li class="item{=index +1}" data-id="{=movie.movieCode}" data-detail="{=movie.movieCode}" data-reserve="{=movie.movieCode}" onmouseover="jindo.$Element('downloadTooltip{=index+1}').show();" onmouseout="jindo.$Element('downloadTooltip{=index+1}').hide();">
    			<div class="obj_off tab4">
    				<a href="https://serieson.naver.com/tvstore/detail.nhn?mcode={=movie.movieCode}" target="_blank"  onfocus="jindo.$Element('downloadTooltip{=index+1}').show();oTimer.abort();" onblur="jindo.$Element('downloadTooltip{=index+1}').hide();movieChart.restartTimer();"><span class="rank"><em>{=index +1}위</em></span>
    					{if movie.adult}
    						<span class="ico_rating_19">청소년 유해물</span>
    					{elseif movie.lastKoreanGrade != null}
    						{js movieChart.getGradeIcon(=movie.lastKoreanGrade.code)}
    					{/if}
    					<span class="mask"></span> {if movie.salePossibleYn == true}<span class="purchase">구매</span>{/if} {if movie.lendingPossibleYn == true}<span class="rental">대여</span>{/if}
    					<img src="https://movie-phinf.pstatic.net{=movie.posterImageUrl}?type=f125" alt="{js movieChart.replaceDoubleQuotationForHTML(=movie.movieTitle)}" width="125" height="179" onerror="this.src='https://ssl.pstatic.net/static/movie/2012/06/dft_img125x179.png'">
    					<span class="baseplate r">
    						<span class="spr stic_down l"><em>판매율</em></span>
    						<strong class="l">{js movieChart.numberFont(=movie.formattedSaleRate, 'rate')}<span class="char rate_pct"><em>%</em></span></strong>
    					</span>
    				</a><!-- N=a:run.da,r:{=index + 1},i:{=movie.movieCode} -->
    			</div>
    			<div id="downloadTooltip{=index+1}" class="obj_con" style="display:none">
    				<div class="obj_on{js movieChart.tooltipLengthOver(=movie.movieTitle)} {if (index+1)%5 == 0}rt{/if}">
    					<div class="tooltip">
    						<span class="top"></span>
    						<p class="mv_title">{=movie.movieTitle}</p>
    						<span class="bottom"></span><span class="bottom_r"></span>
    					</div>
    				</div>
    			</div>
    		</li>
    	{/for}
    {/if}
    </script>
    
    
    <script type="text/javascript">
    
    
    
    
    
    var flickContents = new Array(6);
    
    
    var htInfo = jindo.m.getDeviceInfo(); 
    var bUseCss3d = jindo.m._isUseCss3d() || (htInfo.galaxyS2 && (htInfo.version >= "4.0.3"));
    var oFlicking = new jindo.m.CircularFlicking(jindo.$('mflick'),{
    	nDuration : 100,
    	bHorizontal : true,
        sClassPrefix : 'flick-',
        nFlickThreshold : 40,
        nTotalContents : 6,
        bUseCss3d : bUseCss3d
    }).attach({
    
    	// 타이머 정지 및 메뉴 하이라이팅
    	'beforeFlicking' : function(oCustomEvt) {
    		oTimer.abort();
    
    		var index = oCustomEvt.nContentIndex;
    		var nextIndex = movieChart.getNextIndex(index);
    		var previousIndex = movieChart.getPreviousIndex(index);
    
    		if (oCustomEvt.bLeft) {
    			movieChart.setMenuHighlighting(nextIndex);
    		} else {
    			movieChart.setMenuHighlighting(previousIndex);
    		}
    		
    		
            this.getPanelElement().css('display', 'block');
            this.getRightPanelElement().css('display', 'block');
            this.getLeftPanelElement().css('display', 'block');
    	},
    	
    	// 플리킹처리 및 타이머 재시작 및 캡션내용 변경
    	'afterFlicking' : function(oCustomEvt){
    		
    		if (oCustomEvt.bLeft) {
    			var type = movieChart.movieChartTab[oCustomEvt.nContentRightIndex];
    			
    			// 플리킹 저장변수에 이미 데이터가 있다면 저장변수 이용, 없으면 Ajax Call.
    			if (flickContents[oCustomEvt.nContentRightIndex]) {
    				movieChart.movieChartJsonCallBack(null, flickContents[oCustomEvt.nContentRightIndex], type, oCustomEvt.nContentRightIndex, oCustomEvt.nPanelRightIndex);
    			} else {
    				movieChart.ajaxCall(movieChart.movieChartJsonUrl, type, oCustomEvt.nContentRightIndex, oCustomEvt.nPanelRightIndex);
    			}
    			
    		} else {
    			var type = movieChart.movieChartTab[oCustomEvt.nContentLeftIndex];
    			
    			// 플리킹 저장변수에 이미 데이터가 있다면 저장변수 이용, 없으면 Ajax Call.
    			if (flickContents[oCustomEvt.nContentLeftIndex]) {
    				movieChart.movieChartJsonCallBack(null, flickContents[oCustomEvt.nContentLeftIndex], type, oCustomEvt.nContentLeftIndex, oCustomEvt.nPanelLeftIndex);
    			} else {
    				movieChart.ajaxCall(movieChart.movieChartJsonUrl, type, oCustomEvt.nContentLeftIndex, oCustomEvt.nPanelLeftIndex);
    			}
    		}
    
    		
    		this.getRightPanelElement().css('display', 'none');
    		this.getLeftPanelElement().css('display', 'none');
    		
    		movieChart.restartTimer();
    	}
    });
    
    //[MOVIEOP-5993] [모바일웹] Android 공통댓글 이전/다음 버튼 클릭시 포커싱 유지(PC 환경에서는 Flicking 되지 않도록 수정.)
    var osInfo = jindo.$Agent().os();
    if(osInfo.win || osInfo.mac || osInfo.linux) {
    	oFlicking.attach({
    		'touchStart' : function(oCustomEvt){
    			oCustomEvt.stop();
    			}
    	});
    }
    
    
    var oTimer = new jindo.Timer();
    
    
    var movieChart = {
    
    		movieChartDefaultJsonUrl : "/movieChartDefaultJson.naver",
    		movieChartJsonUrl : "/movieChartJson.naver",
            eTabtoKoTab : {
    		    "RESERVE": "예매순",
                "CURRENT": "현재상영작",
                "COMMING": "개봉예정작",
                "POINT": "평점순",
                "BOXOFFICE": "박스오피스",
                "DOWNLOAD": "다운로드순"
            },
    		movieChartTab : new Array("RESERVE", "CURRENT", "COMMING", "POINT", "BOXOFFICE", "DOWNLOAD"),
            extractTabName: function (obj) {
                var keys = Object.keys(obj);
                var i;
    		    for (i = 0; i < keys.length; i++) {
    		        if (keys[i] != "index") {
    		            return this.eTabtoKoTab[keys[i]];
                    }
                }
                return "";
    		},
    		movieChartAllViewUrl : new Array(
    				"/movie/running/current.naver?order=reserve",
    				"/movie/running/current.naver",
    				"/movie/running/premovie.naver?order=reserve",
    				"/movie/running/current.naver?order=point",
    				"/movie/sdb/rank/rboxoffice.naver",
    				"https://serieson.naver.com/movie/top100List.nhn?rankingTypeCode=PC_D"
    		),
    
    		// 개봉예정작 목록의 마지막 영화의 상영관이 없다면, 예매율순 개봉예정작에서 데이터가 부족해서 상영관이 없는 데이터도 채워넣은 경우이기 때문에 더보기 링크 제공하지 않음
    		hasCommingMovieAllViewUrl : true,
    		
    		// domready시 수행
    		init : function() {
    			movieChart.ajaxCall(movieChart.movieChartJsonUrl, movieChart.movieChartTab[0], 0, 0);
    			movieChart.setMenuHighlighting(0);
    			movieChart.startTimer();
    		},
    		
    		// load시 수행
    		load : function() {
    			movieChart.ajaxCall(movieChart.movieChartJsonUrl, movieChart.movieChartTab[1], 1, 1);
    			movieChart.ajaxCall(movieChart.movieChartJsonUrl, movieChart.movieChartTab[movieChart.movieChartTab.length-1], movieChart.movieChartTab.length-1, 2);
    		},
    		
    		// 타이머 재시작
    		restartTimer : function() {
    			
    			if (oTimer.isRunning = true) {
    				oTimer.abort();
    			}
    			
    			oTimer = new jindo.Timer();
    			movieChart.startTimer();
    		},
    		
    		// 타이머 시작
    		startTimer : function() {
    			oTimer.start( function() {
    				oFlicking.moveNext();
    				return true;
    			}, 7000);
    		},
    		
    		// JSON API 호출
    		ajaxCall : function(url, type, index, targetAreaIndex) {
    			var ajax = new jindo.$Ajax(url, { 
    				method : "GET",
    				onload : function(response){
    					if (url == movieChart.movieChartDefaultJsonUrl) {
    						// 풀세팅 
    						movieChart.movieChartDefaultJsonCallBack(response, null, index);
    					} else {
    						// 개별세팅
    						movieChart.movieChartJsonCallBack(response, null, type, index, targetAreaIndex);
    					}
    				}
    			});
    			ajax.header("ajax", "true");
    		    ajax.request({"type":type});
    		},
    
    		// 무비차트 풀세팅 CallBack 함수
    		movieChartDefaultJsonCallBack : function(response, movieChartList, index) {
    
    			if (movieChartList == null) {
    				var jsonData = response.json();
    				movieChartList = jsonData.movieChartList;
    			}
    			
    			var nextIndex = movieChart.getNextIndex(index);
    			var previousIndex = movieChart.getPreviousIndex(index);
    
    			oFlicking.setContentIndex(index);
    			oFlicking.getPanelElement().html(jindo.$Template(movieChart.movieChartTab[index] + "_template").process(movieChartList[0]));
    			oFlicking.getRightPanelElement().html(jindo.$Template(movieChart.movieChartTab[nextIndex] + "_template").process(movieChartList[1]));
    			oFlicking.getLeftPanelElement().html(jindo.$Template(movieChart.movieChartTab[previousIndex] + "_template").process(movieChartList[2]));
                this.setCaptionText(oFlicking.getPanelElement().attr('id'),  this.extractTabName(movieChartList[0]));
                this.setCaptionText(oFlicking.getRightPanelElement().attr('id'), this.extractTabName(movieChartList[1]));
                this.setCaptionText(oFlicking.getLeftPanelElement().attr('id'), this.extractTabName(movieChartList[2]));
    
    			flickContents[index] = movieChartList[0];
    			flickContents[nextIndex] = movieChartList[1];
    			flickContents[previousIndex] = movieChartList[2];
    			
    			if (index == 2) {
    				this.setHasCommingMovieAllViewUrl(movieChartList[0]);
    				movieChart.setMenuHighlighting(index);
    			}
    			
    			
                oFlicking.getPanelElement().css('display', 'block');
                oFlicking.getRightPanelElement().css('display', 'none');
                oFlicking.getLeftPanelElement().css('display', 'none');
    		},
    		
    		// 플리킹 및 좌우 네비게이션 버튼 클릭에 따른 CallBack 함수
    		movieChartJsonCallBack : function(response, movieChartList, type, index, targetAreaIndex) {
    
    			if (movieChartList == null) {
    				var jsonData = response.json();
    				movieChartList = jsonData.movieChartList;
    			}
    
    			jindo.$Element("flick" + targetAreaIndex).html(jindo.$Template(type + "_template").process(movieChartList));
                this.setCaptionText(jindo.$Element("flick" + targetAreaIndex).attr('id'), this.extractTabName(movieChartList));
    			flickContents[index] = movieChartList;
    			
    			if (index == 2) {
    				this.setHasCommingMovieAllViewUrl(movieChartList);
    			}
    
    			
    			oFlicking.getPanelElement().css('display', 'block');
    			oFlicking.getRightPanelElement().css('display', 'none');
    			oFlicking.getLeftPanelElement().css('display', 'none');
    		},
    		
    		// 무비차트 풀세팅 호출
    		fullSettingMovieChart : function(index) {
    			movieChart.setMenuHighlighting(index);
    			
    			var nextIndex = movieChart.getNextIndex(index);
    			var previousIndex = movieChart.getPreviousIndex(index);
    
    			// 저장변수에 데이터가 이미 있다면 저장변수 이용, 아니면 Ajax Call.
    			if (flickContents[index] && flickContents[nextIndex] && flickContents[previousIndex]) {
    				var movieChartList = new Array(flickContents[index], flickContents[nextIndex], flickContents[previousIndex]);
    				movieChart.movieChartDefaultJsonCallBack(null, movieChartList, index);
    			} else {
    				movieChart.ajaxCall(movieChart.movieChartDefaultJsonUrl, movieChart.movieChartTab[index], index);
    			}
    		},
    		
    		// 메뉴 하이라이팅 처리
    		setMenuHighlighting : function(index) {
    
    			// 탭메뉴 하이라이팅
    			for (i=0; i<movieChart.movieChartTab.length; i++) {
    				jindo.$Element(movieChart.movieChartTab[i] + "_tab").removeClass("on");
    			}
    			jindo.$Element(movieChart.movieChartTab[index] + "_tab").addClass("on");
    			
    			// 전체보기 URL 세팅
    			jindo.$("movieChartAllView").href = movieChart.movieChartAllViewUrl[index];
    			
    			// [다운로드순]일 경우, 전체보기 아이콘이 다르다. (새창)
    			if (movieChart.movieChartTab[index] == "DOWNLOAD") {
    				jindo.$Element(jindo.$$.getSingle(".all_view_go")).show();
    				jindo.$("movieChartAllView").target = "_blank";
    				jindo.$Element(jindo.$$.getSingle(".all_view_go")).addClass("dwn");
    			}
    			// [개봉예정작]일 경우 예매율순 개봉예정작에서 데이터가 부족해서 채워넣은 경우이면 전체 보기 링크를 보여주지 않는다. 
    			else if (movieChart.movieChartTab[index] == "COMMING" && !this.hasCommingMovieAllViewUrl) {
    				jindo.$Element(jindo.$$.getSingle(".all_view_go")).hide();
    			}
    			else {
    				jindo.$Element(jindo.$$.getSingle(".all_view_go")).show();
    				jindo.$("movieChartAllView").target = "_self";
    				jindo.$Element(jindo.$$.getSingle(".all_view_go")).removeClass("dwn");
    			}
    
    			// 최종상태(index)가 정해지는 부분에 추가
    
    			
    		},		
    
    		// 웹접근성을 위한 caption안내
    		setCaptionText: function(id, tabName) {
                switch (id) {
                    case 'flick0':
                        jindo.$Element(jindo.$$.getSingle("#pannel0")).text(tabName);
                        break;
                    case 'flick1':
                        jindo.$Element(jindo.$$.getSingle("#pannel1")).text(tabName);
                        break;
                    case 'flick2':
                        jindo.$Element(jindo.$$.getSingle("#pannel2")).text(tabName);
                        break;
                }
    		},
    		// 두개의 포토인프라도메인을 분산해서 제공 
    		getPhotoInfraImageDomain : function() {
    			var photoInfraImageDomains = new Array("http://movie.phinf.naver.net", "http://movie2.phinf.naver.net");
    			return photoInfraImageDomains[Math.floor((Math.random()*(2)))];
    		},
    		
    		// 따옴표 escape 처리
    		replaceDoubleQuotationForHTML : function(title) {
    			if (title == null) {
    				return null;
    			}
    
    			var result = "";
    			for (i=0; i<title.length; i++) {
    				var tmpChar = title.charAt(i);
    				if (tmpChar == "\"") {
    					result += "&quot;";
    				} else if (tmpChar == "\n" || tmpChar == "\r") {
    					result += "";
    				} else {
    					result += tmpChar;
    				}
    			}
    			return result;
    		},
    		
    		// 이미지폰트 정의
    		numberFont : function(value, charName) {
    			var result = "";
    
    			if (value == 'undefined') {
    				value = "0";
    			}
    			
    			for (i=0; i<value.length; i++) {
    				var tmpChar = value.charAt(i);
    
    				result += '<span class="char ' + charName + '_';
    				if (tmpChar == ".") {
    					result += "dot";
    				} else if (tmpChar == ",") {
    					result += "comma";
    				} else {
    					result += "num" + tmpChar;
    				}
    				result += '"><em>' + tmpChar + '</em></span>';
    			}
    
    			return result;
    		},
    		
    		// 포스터 툴팁 길이제한 확인
    		tooltipLengthOver : function(value) {
    			if (value != null && value.length > 18) {
    				return " br";
    			}
    			return "";
    		},
    		
    		// 플리킹영역 다음 index를 얻는다.
    		getNextIndex : function(index) {
    			var nextIndex = index + 1;
    			if (nextIndex > movieChart.movieChartTab.length - 1) {
    				nextIndex = 0;
    			}
    			return nextIndex;
    		},
    		
    		// 플리킹영역 이전 index를 얻는다.
    		getPreviousIndex : function(index) {
    			var previousIndex = index - 1;
    			if (previousIndex < 0) {
    				previousIndex = movieChart.movieChartTab.length - 1;
    			}
    			return previousIndex;
    		}, 
    		
    		// 개봉예정작의 전체보기 버튼 노출 여부
    		setHasCommingMovieAllViewUrl : function(movieList) {
    			if (movieList.COMMING[movieList.COMMING.length - 1].theater == 0) {
    				this.hasCommingMovieAllViewUrl = false;	
    			} else {
    				this.hasCommingMovieAllViewUrl = true;	
    			}
    		},
    
    		// 등급 아이콘 html을 얻는다.
    		getGradeIcon : function(gradeCode) {
    			var result = '<span class="ico_rating_';
    			if (gradeCode == "1001001") {
    				result += 'all">전체 관람가'
    			} else if (gradeCode == "1001002") {
    				result += '12">12세 관람가'
    			} else if (gradeCode == "1001003") {
    				result += '15">15세 관람가'
    			} else if (gradeCode == "1001004") {
    				result += '18">청소년 관람불가'
    			} else if (gradeCode == "1001005") {
    				result += 'restricted">제한 상영가'
    			} else {
    				return "";
    			}
    
    			result += '</span>'	;
    
    			return result;
    		}
    };
    
    
    var HomeMovieReviewAccordion = jindo.$Class({
    	$init : function(sClassName) {
    		_self = this;
    		this._wel = jindo.$Element("movieReview");
    		this._welList = this._wel.query ("ul.lst_con." + sClassName);
    		
    		this._wel.delegate(
    				"mouseover",
    				"._select_title",
    				jindo.$Fn(this._onMouseOverItem, this).bind()
    		);
    		
    		jindo.$A(jindo.$ElementList('._select_title_anchor').$value()).forEach(function(element, index, array) {
    			jindo.$Fn(_self._onMouseOverItem, _self).attach(element, "focus");
    		});
    	},
    	
    	_onMouseOverItem : function (we) {
    		we.stopDefault();
    		var nIndex = Number(jindo.$Element(we.element).data('index'));
    		
    		this.openReview(nIndex);
    	},
    	
    	openReview : function (nIndex) {
    		var aEls = this._welList.queryAll("li ! li");
    		
    		// 해당하는 항목만 <li class="on">
    		for (var i = 0; i < aEls.length; i++) {
    			aEls[i].cssClass("on", nIndex == i);
    		}
    	},
    	
    	showRandomMovie : function () {
    		var randNo = Math.floor(4 * Math.random());
    		this.openReview(randNo);
    	}
    });
    
    
    
    var oFirstHomeMovieReviewAccordion = new HomeMovieReviewAccordion("first");
    
    
    jindo.$Fn(function() {oFirstHomeMovieReviewAccordion.showRandomMovie();}).attach(document, "domready");
    
    jindo.$Fn(function() {movieChart.init();}).attach(document, "domready");
    jindo.$Fn(function() {movieChart.load();}).attach(window, "load");
    jindo.$Fn(function(evt){evt.stop(); oFlicking.movePrev();}, this).attach(jindo.$("flick_prev"),"click");
    jindo.$Fn(function(evt){evt.stop(); oFlicking.moveNext();} ,this).attach(jindo.$("flick_next"),"click");
    
    var nsc = "movie.home";
    </script>
    	</div>
    	<!-- //container -->
    	
    	<!-- footer -->
    	
    
    
    
    <div id="footer">
    	<div class="in_footer">
    		<div class="foot_con">
    				<ul>
    					<li class="first"><a href="http://www.naver.com/rules/service.html" target="_blank">이용약관</a><!-- N=a:fot.agreement --></li>
    					<li><a href="http://www.naver.com/rules/privacy.html" target="_blank"><strong>개인정보처리방침</strong></a><!-- N=a:fot.privacy --></li>
    					<li><a href="http://www.naver.com/rules/disclaimer.html" target="_blank">책임의 한계와 법적고지</a><!-- N=a:fot.disclaimer --></li>
    					<li><a href="https://help.naver.com/support/service/main.nhn?serviceNo=800" target="_blank">영화 고객센터</a><!-- N=a:fot.help --></li>
    				</ul>
    				<p class="info">본 콘텐츠의 저작권은 저작권자 또는 제공처에 있으며, 이를 무단 이용하는 경우 저작권법 등에 따라 법적 책임을 질 수 있습니다.</p>
    				<p class="info">
    					사업자등록번호 : 220-81-62517<span>통신판매업 신고번호</span> : 경기성남 제 2006 - 692호<span>대표이사 : 한성숙</span><span><a href="http://www.ftc.go.kr/info/bizinfo/communicationList.jsp">사업자등록정보 확인</a><!-- N=a:fot.bizinfo --></span><br>
    					주소 : 경기도 성남시 분당구 불정로 6 네이버 그린팩토리 <span>대표전화 : 1588-3820</span>
    				</p> 
    				<address>
    					<a href="https://www.navercorp.com/" target="_blank" class="logo"><img src="https://ssl.pstatic.net/static/movie/2013/07/logo_naver.png" width="63" height="11" alt="NAVER"></a><!-- N=a:fot.nhn -->
    					<em>Copyright ©</em>
    					<a href="https://www.navercorp.com/" target="_blank">NAVER Corp.</a><!-- N=a:fot.corp -->
    					<span>All Rights Reserved.</span>
    				</address>
    		</div>
    	</div>
    </div>
    
    
    
    
    
    
    
    
    <script type="text/javascript">
    
    if (false) {
    	var alertType = "NONE";
    	var koreanTitle = "";
    	var movieCode = "0";
    	var userReserveCount = "0";
    	var todayDatetime = "20210817172555";
    	var endDatetimeAfterTwoDays = "00000000000000";
    	
    	
    	if (movieCode > 0) {
    		openWriteActualPointAlert (alertType, koreanTitle, movieCode, userReserveCount, todayDatetime, endDatetimeAfterTwoDays);
    	}
    }
    
    function openWriteActualPointAlert (alertType, koreanTitle, movieCode, count, today, endDate) {
    	if (alertType == "ONE") {
    		setCookieLastUserReserveDate(today, endDate);
    		if (confirm("관람하신 " + koreanTitle + "에\n평점 등록 시 네이버페이 포인트 500원 적립!\n지금 평점쓰기 메뉴로 이동하시겠습니까?")) {
    			top.location.href = "https://movie.naver.com/movie/bi/mi/point.naver?code=" + movieCode;
    		}
    	} else if (alertType == "MORE") {
    		setCookieLastUserReserveDate(today, endDate);
    		if (confirm("관람하신 작품에 평점을 등록해주세요\n작품당 네이버페이 포인트 500원씩 적립!\n평점 미등록작 리스트를 확인하시겠습니까?")) {
    			top.location.href = "http://ticket.movie.naver.com/Order/OverdueList.aspx";
    		}
    	}
    }
    
    function setCookieLastUserReserveDate(today, endDate) {
    	var cookieForNotOpenActualPointPopup = jindo.$Cookie();
    	
    	
    	cookieForNotOpenActualPointPopup.remove("lastUserReserveDatetime");
    	cookieForNotOpenActualPointPopup.remove("lastUserReserveCheckDatetime");
    	
    	cookieForNotOpenActualPointPopup.set("lastUserReserveDatetime", endDate, 9999, "movie.naver.com");
    	cookieForNotOpenActualPointPopup.set("lastUserReserveCheckDatetime", today, 9999, "movie.naver.com");
    }
    
    </script>
    
    
    
    
    
    
    
    
    <script type="text/javascript">
    	
    		
    		
    		
    		
    			var alertMessage = "지원되지 않는 브라우저로 서비스 이용에 제한이 있습니다.";
    		
    	
    
    	function getBrowser() {
    		var ua = navigator.userAgent;
    		if (/NAVER/.test(ua)) {
    			return "NAVER_APP";
    		} else if (/IEMobile/.test(ua)) {
    			return "INTERNET_EXPLORER_MOBILE";
    		} else if (/MSIE/.test(ua) || /Trident/.test(ua)) {
    			return "INTERNET_EXPLORER";
    		} else if (/Firefox/.test(ua)) {
    			return "FIREFOX";
    		} else if (/Opera\//.test(ua) || /OPR\//.test(ua)) {
    			return "OPERA";
    		}  else if (/Swing\//.test(ua)) {
    			return "SWING";
    		} else if (/Chrome\//.test(ua) || /CriOS\//.test(ua)) {
    			return "CHROME";
    		} else if (/BAND\//.test(ua)) {
    			return "BAND_APP";
    		} else if (/FBAN\/FBIOS/.test(ua)) {
    			return "FACEBOOK_APP";
    		} else if (/Twitter/.test(ua)) {
    			return "TWITTER_APP";
    		} else if (/KAKAOTALK/.test(ua)) {
    			return "KAKAOTALK_APP";
    		} else if (/Android/.test(ua) && /Safari/.test(ua)) {
    			return "ANDROID_INTERNET_APP";
    		} else if (/Safari/.test(ua)) {
    			return "SAFARI";
    		}
    
    		return "";
    	}
    
    	if (getBrowser() === "UNKNOWN" && jindo.$Cookie().get("notSupportBrowserAlert") != 'true') {
    		alert(alertMessage);
    		jindo.$Cookie().set("notSupportBrowserAlert", "true", "9999", "movie.naver.com");
    	}
    
    
    </script>
    
    
    	<!-- //footer -->
    </div>
    <script type="text/javascript">
    
    jindo.$Fn(function (we) {
    
    	// 상단 검색영역
    	var oSearch = new nhn.movie.Search({
    		area : "jSearchArea",
    		autosearch : "https://auto-movie.naver.com/ac?q_enc=UTF-8&st=1&r_lt=1&n_ext=1&t_koreng=1&r_format=json&r_enc=UTF-8&r_unicode=0&r_escape=1&q=",
    		movelink : "/movie/bi/mi/basic.naver?code=",
    		peoplelink : "/movie/bi/pi/basic.naver?code="
    	});
    
        // 좌측 LNB
        var oLNB = new nhn.movie.LNB();
    	if( typeof oViewMode != "undefined") {
    		oViewMode.attach('change', jindo.$Fn(oLNB.update, oLNB).bind());
    	}
    
        //영화검색 결과에서 포커스 아웃될 경우, 검색 결과를 지우도록 변경.
        jindo.$Element("lnb_gonaver").attach("focus",function(e){
        	
        	jindo.$Element('search_placeholder').attr({
        		"style" : "display: inline;"
        	})
        	jindo.$Element('ipt_tx_srch').$value().value="";
        	if(jindo.$Element("jAutoComplate") != null){
        		jindo.$Element("jAutoComplate").hide();
        	}
        });
    }).attach(document, 'domready');
    
    //LCS
    jindo.$Fn(function() {
        try{ lcs_do(); } catch(e){}
    }).attach(window, "pageshow");
    
    
    </script>
    <script type="text/javascript">
    	//nClick 초기화 영역
    	//클릭로그 집계 코드 추가
    	var ccsrv="cc.naver.com";
    	var nclk_evt = 1;
    	
    	nclk_do();
    	//nClick 초기화 영역 끝
    </script>
    </body>
    </html>
    


```python
type(text)
```




    str




```python

```
