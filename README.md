# STARLAB

**차례**
1. [레드햇 엔터프라이즈 리눅스](README.md#1-레드햇-엔터프라이즈-리눅스)
2. [앤서블 오토메이션 플랫폼](README.md#2-앤서블-오토메이션-플랫폼)
3. [오픈시프트 가상화](README.md#3-오픈시프트-가상화)
4. [오픈스택 서비스](README.md#4-오픈스택-서비스)
5. [RHEL AI](README.md#5-rhel-ai)
99. [참조](README.md#99-참조)
<br>
<br>

## 1. 레드햇 엔터프라이즈 리눅스

Red Hat Enterprise Linux (RHEL)는 엔터프라이즈 환경을 위한 안정성 / 성능 / 보안을 제공하는 리눅스 운영체제 입니다.

### 1.1 RHEL 기능 소개

* [Pacemaker 설치 및 구성](https://github.com/starlab3030/pacemaker)
<br>
<br>

## 2. 앤서블 오토메이션 플랫폼

Ansible Automation Platform (AAP)는 미션 크리티컬한 IT 환경에 고객의 요구와 서비스에 맞게 안전하고 유연한 인프라 확장 및 자동화 관리를 제공하는 플랫폼 입니다.

* [AAP 2.5 설치](https://github.com/starlab3030/aap-instalation)
<br>
<br>

## 3. 오픈시프트 가상화

OpenShift Virtualization (virt)는 오픈시프트를 기반으로 클라우드-네이티브 가상화를 제공하는 플랫폼 입니다.

* [오픈시프트 가상화 로드쇼](https://github.com/starlab3030/openshift-virt-lab/tree/main/openshift)
<br>
<br>

## 4. 오픈스택 서비스

Red Hat OpenStack Services on OpenShift (RHOSO)는 오픈시프트 상에 오픈스택 컨트롤-플레인을 설치하고, RHEL 기반의 컴퓨트 노드를 구성할 수 있는 서비스 입니다.

### 4.1 RHOSO 설치

* 기본적인 방식으로 오픈시프트 상에서 오픈스택 설치
  + 오픈스택 서비스 설치 사전 준비, 설치까지 오픈시프트가 제공하는 CLI(oc 명령어) 및 GUI를 통해 설치
  + 오프스택을 설치하는 기본적인 방법
* ArgoCD를 통한 GitOps 형태로 오픈스택 설치
  + 오프스택 설치에 필요한 리소스를 GitHub에 YAML로 구성 후, ArgoCD 앱을 생성하여 설치
  + 오픈시프트가 제공하는 GitOps를 통해 빠르고 쉽게 설치 가능

#### 4.1.1 기본 설치 

1. [사전 준비](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab/pre-requisite-ops.md)
2. [오픈스택 서비스 오퍼레이터 설치](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab/install-oso-operators.md)
3. [오픈스택 서비스 보안 접근 구성](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab/provide-secure-access-to-rhoso.md)
4. [오픈스택 서비스 네트워크 구성](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab/prepare-openshfit-for-rhoso-network-isolation.md)
5. [오픈스택 서비스 컨트롤-플레인 생성](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab/create-oso-ctl-plane.md)
6. [오픈스택 데이터-플레인 구성](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab/configure-data-plane.md)
7. [오픈스택 접속](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab/access-openstack.md)
8. [오픈스택 노드 확장](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab/scale-out-compute.md)

#### 4.1.2 ArgoCD를 기반으로 오픈스택 설치

1. [ArgoCD 설치](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab-via-argocd/install-argocd.md)
2. [사전 준비](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab-via-argocd/pre-requisite-ops-via-argocd.md)
3. [오픈스택 서비스 오퍼레이터 설치](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab-via-argocd/install-oso-operators-via-argocd.md)
4. [오프스택 서비스 네트워크 구성](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab-via-argocd/prepare-openshfit-for-rhoso-network-isolation-via-argocd.md)
5. [오픈스택 서비스 컨트롤-플레인 생성](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab-via-argocd/create-oso-ctl-plane-via-argocd.md)
6. [오픈스택 데이터-플레인 구성](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab-via-argocd/configure-data-plane-via-argocd.md)
7. [오픈스택 노드 확장](https://github.com/starlab3030/rhoso-temp/blob/main/beta-lab-via-argocd/scale-out-compute.md)
<br>
<br>

## 5. RHEL AI

RHEL AI는 엔터프라이즈 환경에서 쉽고 빠르게 AI를 도입하여 도메인 지식을 가지고 고객에 환경 및 요구 사항에 맞추어, LLM을 커스터마이징하고 서비스를 할 수 있도록 도와주는 플랫폼 입니다.

고객은 출시된 모델을 기반으로 AI 앱을 연동하여 서비스를 제공할 수 있습니다.

### 5.1 RHEL AI 기술

* [RHEL AI](https://github.com/starlab3030/rhel-ai)

* `STARLAB3030`을 위한 AI
  + [허깅페이스](https://github.com/starlab3030)
  + [마크다운 문서](https://github.com/starlab3030/knowledges_for_instructlab)
  + [택소노미 트리](https://github.com/starlab3030/taxonomy_for_instructlab)
<br>

### 5.2 AI를 위한 교육

|세션|항목|
|:---|:---|
|RHEL AI 101|* [NVIDIA 소개 및 특징](https://github.com/starlab3030/rhel-ai/blob/main/nvidia_gpus/nvidia_gpu_features.md)<br>* [RHEL AI 소개](https://github.com/starlab3030/rhel-ai/blob/main/contents/instroduction_of_rhel_ai.md)<br>* [RHEL AI 설치 & 관리](https://github.com/starlab3030/rhel-ai/blob/main/contents/manage_life-cycle_of_rhel_ai.md)|
|RHEL AI 201|* [RHEL AI 기본 설정](https://github.com/starlab3030/rhel-ai/blob/main/contents/rhel_ai.md)<br>* [기술 및 지식](https://github.com/starlab3030/rhel-ai/blob/main/contents/skills_and_knowledges.md)<br>* [커스텀 LLM 구성](https://github.com/starlab3030/rhel-ai/blob/main/contents/generate_custom_llm.md)|
|RHEL AI 301|* [커스텀 LLM 생성](https://github.com/starlab3030/rhel-ai/blob/main/sample_tests/custom_llm_with_dgx-h100.md)<br>* [다양한 모델 훈련 변수](https://github.com/starlab3030/rhel-ai/blob/main/sample_tests/train_llm_with_various_vars.md)|

<br>

<!---
<table>
  <tr>
    <th>세션</th>
    <th>항목</th>
  </tr>
  <tr>
    <td>RHEL AI 101</td>
    <td>
      <ul>
        <li><a href=https://github.com/starlab3030/rhel-ai/blob/main/nvidia_gpus/nvidia_gpu_features.md>NVIDIA 소개 및 특징</a></li>
        <li><a href=https://github.com/starlab3030/rhel-ai/blob/main/contents/instroduction_of_rhel_ai.md>RHEL AI 소개</a></li>
        <li><a href=https://github.com/starlab3030/rhel-ai/blob/main/contents/manage_life-cycle_of_rhel_ai.md>RHEL AI 설치 & 관리</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>RHEL AI 201</td>
    <td>
      <ul>
        <li><a href=https://github.com/starlab3030/rhel-ai/blob/main/contents/rhel_ai.md>RHEL AI 기본 설정</a></li>
        <li><a href=https://github.com/starlab3030/rhel-ai/blob/main/contents/skills_and_knowledges.md>기술 및 지식</a></li>
        <li><a href=https://github.com/starlab3030/rhel-ai/blob/main/contents/generate_custom_llm.md>커스텀 LLM 구성</a></li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>RHEL AI 301</td>
    <td>
      <ul>
        <li><a href=https://github.com/starlab3030/rhel-ai/blob/main/sample_tests/custom_llm_with_dgx-h100.md>커스텀 LLM 생성</a></li>
        <li><a href=https://github.com/starlab3030/rhel-ai/blob/main/sample_tests/train_llm_with_various_vars.md>다양한 모델 훈련 변수</a></li>
      </ul>
    </td>
  </tr>
</table>
--->

### 5.3 커뮤니티 InstructLAB

CY24 RHSC 키노트 세션 데모
1. [LLM과 InstructLAB](https://github.com/starlab3030/rhel-ai/blob/main/rhsc-demo/introdution-of-lab.md)
2. [InstructLAB 기반 모델 관리](https://github.com/starlab3030/rhel-ai/blob/main/rhsc-demo/start-with-instructlab.md)
3. [AI를 보험 앱에 통합하기](https://github.com/starlab3030/rhel-ai/blob/main/rhsc-demo/integrate-ai-into-app.md)
<br>
<br>

## 99. 참조

<!---
### 99.1 RHEL을 위한 참조 링크

*차후 업데이트*
<br>

### 99.2 AAP를 위한 참조 링크

*차후 업데이트*
<br>

### 99.3 오픈시프트 가상화를 위한 참조 링크

*차후 업데이트*
<br>

### 99.4 RHOSO를 위한 참조 링크

*차후 업데이트*
<br>
--->

### 99.5 RHEL AI를 위한 참조 링크

#### 99.5.1 커스텀 LLM을 위한 링크

**허깅 페이스**
* [STARLAB3030](https://huggingface.co/starlab3030)

**Git 리포지토리**
* [지식 관련 마크다운 문서](https://github.com/starlab3030/knowledges_for_instructlab)
* [택소노미 트리](https://github.com/starlab3030/taxonomy_for_instructlab)

#### 99.5.2 외부 링크

**InstructLAB 커뮤니티**
* [InstructLAB의 *git* 리포지토리](https://github.com/instructlab)
  + [CLI에 기여](https://github.com/instructlab/instructlab/blob/main/CONTRIBUTING/CONTRIBUTING.md)
  + [NVIDIA 리눅스에 설치](https://docs.instructlab.ai/getting-started/linux_nvidia/)
* [InstructLAB 문서](https://docs.instructlab.ai/)
  + [대시보드 - 택소노미 트리에 기여](https://ui.instructlab.ai/)
    - [기술 기여](https://ui.instructlab.ai/contribute/skill)
    - [지식 기여](https://ui.instructlab.ai/contribute/knowledge)
  + [택소노미 기여 가이드](https://docs.instructlab.ai/taxonomy/upstream/contribution_guidelines/)
    - [기술 기여 가이드](https://docs.instructlab.ai/taxonomy/upstream/skills_contribution_details/)
    - [지식 기여 가이드](https://docs.instructlab.ai/taxonomy/upstream/knowledge_contribution_details/)
<br>

**모델과 채팅**
* [Granite 모델](https://ui.instructlab.ai/playground/chat)
<br>

**IBM Granite 커뮤니티**
* [IBM Granite의 *git* 리포지토리](https://github.com/ibm-granite)
<br>
<br>

------

***Powered By Shadowman*** &nbsp;&nbsp;[HuggingFace](https://huggingface.co/starlab3030)&nbsp;&nbsp;[Blog](https://blog.naver.com/dark_selee) [<img src="images/youtube.png" width="21px" title="100px" alt="유투브"/>](https://www.youtube.com/@starlab3030) &nbsp;&nbsp; [<img src="images/github-mark.svg" width="21px" title="100px" alt="것허브"/>](https://github.com/starlab3030/starlab3030.github.io)
