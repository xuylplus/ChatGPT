<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="icon" type="images/x-icon" href="../static/images/favicon.ico">
    <link rel="stylesheet" href="../static/css/bootstrap.min.css">
    <link rel="stylesheet" href="../static/font-awesome/css/font-awesome.min.css">
    <link rel="stylesheet" href="../static/css/github-dark-dimmed.min.css">
    <link rel="stylesheet" href="../static/css/style.css">
    <title>ChatGPT-website</title>
</head>
<body>
  <div class="container">
    <div class="row">
      <div class="box col-xs-12">
        <div class="title">
            <h2 class="text-center"><span style="margin-right: 10px;"><i class="fa fa-optin-monster fa-lg" aria-hidden="true"></i></span>ChatGPT-website</h2>
        </div>
        <div class="answer">
          <div class="tips">
          </div>
          <div id="chatWindow"></div>
          <div class="function">
            <div class="others">
              <div class="left">
                <div class="settings common dropup">
                  <a class="dropdown-toggle icon-style" id="dropdownMenu" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false" title="设置">
                    <i class="fa fa-cogs fa-lg" aria-hidden="true"></i>
                  </a>
                  <div class="dropdown-menu" style="padding:0;" onclick="event.stopPropagation()">
                    <div class="settings-common">
                      <span><i class="fa fa fa-linode fa-lg" aria-hidden="true"></i>&nbsp; 主题</span>
                      <select class="form-control ipt-common theme">
                        <option value="light">light</option>
                        <option value="gray">gray</option>
                        <option value="light-red">light-red</option>
                        <option value="light-blue">light-blue</option>
                        <option value="light-purple">light-purple</option>
                        <option value="light-green">light-green</option>
                        <option value="light-yellow">light-yellow</option>
                      </select>
                    </div>
                    <div class="settings-common">
                      <span><i class="fa fa-key fa-lg" aria-hidden="true"></i>&nbsp; OpenAI Key</span>
                      <input type="text" class="form-control ipt-common api-key" placeholder="可用自己的api key">
                    </div>
                    <div class="settings-common">
                      <span><i class="fa fa-reddit-alien fa-lg" aria-hidden="true"></i>&nbsp; OpenAI 模型</span>
                      <select class="form-control ipt-common model">
                        <option value="gpt-3.5-turbo">gpt-3.5-turbo</option>
                        <option value="gpt-4">gpt-4</option>
                      </select>
                    </div>
                    <div class="settings-common">
                      <span><i class="fa fa-floppy-o fa-lg" aria-hidden="true"></i>&nbsp; 记录对话内容，刷新不会消失</span>
                      <div class="chck-btn">
                        <input id="chck-1" type="checkbox">
                        <label for="chck-1" class="check-trail">
                        <div class="check-handler"></div>
                        </label>
                      </div>
                    </div>
                    <div class="settings-common">
                      <span><i class="fa fa-retweet fa-lg" aria-hidden="true"></i>&nbsp; 开启连续对话，加倍消耗tokens</span>
                      <div class="chck-btn">
                        <input id="chck-2" type="checkbox">
                        <label for="chck-2" class="check-trail">
                        <div class="check-handler"></div>
                        </label>
                      </div>
                    </div>
                    <div class="settings-common">
                    </div>
                  </div>
                </div>
              </div>
              <div class="center">
                <div class="stop common">
                  <a class="icon-style stop-icon" title="停止响应" style="text-decoration: none;"><i class="fa fa-stop-circle-o fa-lg" aria-hidden="true"></i> 停止</a>
                </div>
              </div>
              <div class="right">
                <div class="screenshot common">
                  <a class="icon-style" title="截图保存对话"><i class="fa fa-file-image-o fa-lg" aria-hidden="true"></i></a>
                </div>
                <div class="delete common">
                  <a class="icon-style" title="删除历史记录"><i class="fa fa-trash-o fa-lg" aria-hidden="true"></i></a>
                </div>
              </div>
            </div>
            <div class="ipt">
              <div class="col-xs-12">
                <textarea id="chatInput" class="form-control" rows="1"></textarea>
              </div>
              <button id="chatBtn" class="btn btn-primary" type="button">Go !</button>
            </div>
          </div>
        </div>
        <footer class="foot" style="margin-top: 20px;">
          <p class="lead text-center">“抢走工作的不会是AI,而是率先掌握AI能力的人”</p>
          <p class="lead text-center">
          </p>
        </footer>
      </div>
    </div>
  </div>
</body>
<script src="../static/js/jquery-2.1.1.js"></script>
<script src="../static/js/bootstrap.min.js"></script>
<script src="../static/js/highlight.min.js"></script>
<script src="../static/js/marked.min.js"></script>
<script src="../static/js/html2canvas.min.js"></script>
<script src="../static/js/custom.js"></script>
</html>
