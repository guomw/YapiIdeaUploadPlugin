### 说明
基于YapiIdeaUploadPlugin 插件基础上，进行二次开发扩展，支持swagger 注解

支持右键项目一键同步Controller文件接口

支持dto mock配置，@ApiModelProperty(example="@mock")

注解使用方式：

字段mock配置：@ApiModelProperty(example="@string")

接口名称：在controller的方法上添加 @ApiOperation("接口名称") or @ApiOperation(value="接口名称")

分组(菜单)名称配置:在controller头上添加 @Api(tags="groupName")

### 使用方式：
.idea/misc.xml 文件中 添加以下配置
````
<!--yapi配置-->
<component name="yapi">
  <option name="projectToken">yapi项目token</option>
  <option name="projectId">项目id</option>
  <option name="yapiUrl">http://yapi.xxxx.com</option>
  <option name="projectType">api</option>
</component>
````