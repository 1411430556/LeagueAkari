<template>
  <div class="single-root">
    <NScrollbar class="outer-wrapper">
      <div class="inner-wrapper">
        <SendableItemEdit />
        <TemplateEdit style="margin-top: 8px" />
        <NCard size="small" style="margin-top: 8px">
          <template #header>
            <span class="card-header-title">{{ t('settings.title') }}</span>
          </template>
          <ControlItem
            :label-width="260"
            :disabled="!as.isAdministrator"
            class="control-item-margin"
            :label="t('settings.cancelShortcut.label')"
            :label-description="t('settings.cancelShortcut.description')"
          >
            <ShortcutSelector
              :shortcut-id="igs.settings.cancelShortcut"
              :target-id="InGameSendRenderer.CANCEL_SHORTCUT_TARGET_ID"
              @update:shortcut-id="(id) => ig.setCancelShortcut(id)"
            />
          </ControlItem>
          <ControlItem
            :label-width="260"
            class="control-item-margin"
            :label="t('settings.sendInterval.label')"
            :label-description="t('settings.sendInterval.description')"
          >
            <NInputNumber
              @update:value="(val) => ig.setSendInterval(val || 65)"
              :value="igs.settings.sendInterval"
              size="small"
              :disabled="!as.isAdministrator"
              :min="10"
              :max="3500"
              :step="15"
              style="width: 120px"
              secondary
              type="warning"
            ></NInputNumber>
          </ControlItem>
        </NCard>
      </div>
    </NScrollbar>
  </div>
</template>

<script setup lang="ts">
import ControlItem from '@renderer-shared/components/ControlItem.vue'
import { useInstance } from '@renderer-shared/shards'
import { useAppCommonStore } from '@renderer-shared/shards/app-common/store'
import { InGameSendRenderer } from '@renderer-shared/shards/in-game-send'
import { useInGameSendStore } from '@renderer-shared/shards/in-game-send/store'
import { useTranslation } from 'i18next-vue'
import { NCard, NInputNumber, NScrollbar } from 'naive-ui'

import ShortcutSelector from '@main-window/components/ShortcutSelector.vue'

import SendableItemEdit from './SendableItemEdit.vue'
import TemplateEdit from './TemplateEdit.vue'

const { t } = useTranslation('renderer', { keyPrefix: 'InGameSend' })

const as = useAppCommonStore()
const igs = useInGameSendStore()
const ig = useInstance(InGameSendRenderer)
</script>

<style lang="less" scoped>
@import '../toolkit-styles.less';

.padding {
  padding: 8px 12px;
}

.addable-tab {
  font-size: 13px;

  .empty {
    filter: opacity(0.8);
  }
}

.empty-placeholder {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 8px;
  font-size: 14px;
  padding: 16px;
  border-radius: 4px;
}

[data-theme='dark'] {
  .empty-placeholder {
    color: #fff8;
    background-color: #ffffff05;
  }
}

[data-theme='light'] {
  .empty-placeholder {
    color: #0008;
    background-color: #00000005;
  }
}
</style>
