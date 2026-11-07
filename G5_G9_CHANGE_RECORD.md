# G5/G9 产品修改记录

- 产品编号：$(@{number=72; product_id=JLZ-EDU-SK-058; chinese_name=员工入职清单; english_name=Employee Onboarding Checklist; repository_name=edu-employee-onboarding-checklist; repository_url=https://github.com/jinlize-tech/edu-employee-onboarding-checklist; product_type=Skill; category_code=06; category=06 人力组织中心; description=员工入职清单。; target_users=System.Object[]; core_input=岗位、入职日期、劳动合同、账号权限、培训安排、导师和试用期目标; main_output=入职清单、责任角色、完成时限、资料收集最小化说明和验收节点; product_risk=过度采集证件或遗漏必要告知; dedup_label=存在部分功能交叉; dedup_note=与通用入职清单相比限定教培岗位和教学系统、排课、家校权限。; development_status=Planned / 待研发; license=Apache-2.0; spec_version=1.0.0; workbuddy_status=PLANNED_FOR_WORKBUDDY}.product_id)
- 产品名称：员工入职清单
- 基线：EDUCATION_BASELINE_V1.0.0
- 基线提交：$BaselineCommit
- 原版本：1.0.0
- 新版本：1.0.1

## 本次修改

1. 强化产品专属执行流程、输入核对和输出验收规则。
2. 新增 scripts/validate_input.js，实际检查必填字段、冲突、未确认数据和敏感信息。
3. 新增正常、缺失、冲突、敏感信息和非法JSON场景输入。
4. 测试升级为 T1–T7 分层并保存逐项检查结果。
5. 安装包加入 Apache-2.0 LICENSE 和 THIRD_PARTY_NOTICES.md。
6. 安装包升级为 1.0.1，加入许可证、第三方声明和输入校验脚本，保留 1.0.0 ZIP。
7. 按本产品冻结规格补充专属处理规则、输入到成果的核对矩阵和去重边界。

## 产品专属增强

- 核心任务：员工入职清单。
- 主要风险：过度采集证件或遗漏必要告知
- 去重边界：与通用入职清单相比限定教培岗位和教学系统、排课、家校权限。

- 从岗位任务、汇报关系、任职资格、协作接口和绩效证据出发，不针对个人画像。
- 区分必要条件与可培养条件，避免歧视性、无限扩张或不相关限制。
- 涉及劳动关系、纪律、薪酬和合规结论时要求专业人员复核。
- 招聘、培训、绩效和入职材料应保留责任人、时间与确认节点。

## 运行边界

- 本地模型行为：NOT_RUNTIME_VERIFIED
- WorkBuddy平台验证：WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- 本轮不执行上传、安装、审核或正式发布。
