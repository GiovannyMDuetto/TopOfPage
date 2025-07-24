# TopOfPage
This is the code for Top of Page component to Figma Make, just copy and paste use as prompt.

```
import svgPaths from "./svg-67thhnvn2m";
import React, { useState } from "react";
import { defineProperties } from "figma:react";

interface InfoIconProps {
  state?: "Default" | "Hover" | "Pressed";
}

function InfoIcon({ state = "Default" }: InfoIconProps) {
  if (state === "Hover") {
    return (
      <div
        className="cursor-pointer relative size-full"
        data-name="State=Hover"
      >
        <div className="absolute inset-0 overflow-clip" data-name="info">
          <div className="absolute inset-[8.333%]" data-name="Vector">
            <svg
              className="block size-full"
              fill="none"
              preserveAspectRatio="none"
              role="presentation"
              viewBox="0 0 15 15"
            >
              <g id="Vector">
                <path d={svgPaths.pa266500} fill="var(--fill-0, #585858)" />
              </g>
            </svg>
          </div>
        </div>
      </div>
    );
  }
  if (state === "Pressed") {
    return (
      <div className="relative size-full" data-name="State=Pressed">
        <div className="absolute inset-0 overflow-clip" data-name="info">
          <div className="absolute inset-[8.333%]" data-name="Vector">
            <svg
              className="block size-full"
              fill="none"
              preserveAspectRatio="none"
              role="presentation"
              viewBox="0 0 15 15"
            >
              <g id="Vector">
                <path d={svgPaths.pa266500} fill="var(--fill-0, #424242)" />
              </g>
            </svg>
          </div>
        </div>
      </div>
    );
  }
  return (
    <div className="relative size-full" data-name="State=Default">
      <div className="absolute inset-0 overflow-clip" data-name="info">
        <div className="absolute inset-[8.333%]" data-name="Vector">
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 15 15"
          >
            <g id="Vector">
              <path d={svgPaths.pa266500} fill="var(--fill-0, #757575)" />
            </g>
          </svg>
        </div>
      </div>
    </div>
  );
}



interface CalendarTodayProps {
  style?: "Filled" | "Outlined" | "Round" | "Sharp" | "Two Tone";
}

function CalendarToday({ style = "Outlined" }: CalendarTodayProps) {
  if (style === "Filled") {
    return (
      <div className="relative size-full" data-name="Style=Filled">
        <div
          className="absolute bottom-[4.167%] left-[8.333%] right-[8.333%] top-[4.167%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            viewBox="0 0 20 22"
          >
            <g id="Vector">
              <path d={svgPaths.p36026d80} fill="var(--fill-0, #1C1C1C)" />
            </g>
          </svg>
        </div>
      </div>
    );
  }
  if (style === "Round") {
    return (
      <div className="relative size-full" data-name="Style=Round">
        <div
          className="absolute bottom-[4.167%] left-[8.333%] right-[8.333%] top-[4.167%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            viewBox="0 0 20 22"
          >
            <g id="Vector">
              <path d={svgPaths.p23caf740} fill="var(--fill-0, #1C1C1C)" />
            </g>
          </svg>
        </div>
      </div>
    );
  }
  if (style === "Sharp") {
    return (
      <div className="relative size-full" data-name="Style=Sharp">
        <div
          className="absolute bottom-[4.167%] left-[8.333%] right-[8.333%] top-[4.167%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            viewBox="0 0 20 22"
          >
            <g id="Vector">
              <path d={svgPaths.p1e3c3180} fill="var(--fill-0, #1C1C1C)" />
            </g>
          </svg>
        </div>
      </div>
    );
  }
  if (style === "Two Tone") {
    return (
      <div className="relative size-full" data-name="Style=Two Tone">
        <div
          className="absolute bottom-[4.167%] left-[8.333%] right-[8.333%] top-[4.167%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            viewBox="0 0 20 22"
          >
            <path
              d={svgPaths.p264aa300}
              fill="var(--fill-0, #1C1C1C)"
              id="Vector"
            />
          </svg>
        </div>
        <div
          className="absolute bottom-[66.667%] left-[16.667%] right-[16.667%] top-[20.875%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            viewBox="0 0 16 3"
          >
            <path
              d="M0 0H16V2.99H0V0Z"
              fill="var(--fill-0, #1C1C1C)"
              id="Vector"
              opacity="0.3"
            />
          </svg>
        </div>
      </div>
    );
  }
  return (
    <div className="relative size-full" data-name="Style=Outlined">
      <div
        className="absolute bottom-[4.167%] left-[8.333%] right-[8.333%] top-[4.167%]"
        data-name="Vector"
      >
        <svg
          className="block size-full"
          fill="none"
          preserveAspectRatio="none"
          viewBox="0 0 20 22"
        >
          <g id="Vector">
            <path d={svgPaths.p30b72580} fill="var(--fill-0, #1C1C1C)" />
          </g>
        </svg>
      </div>
    </div>
  );
}

function PageTitle() {
  return (
    <div
      className="box-border content-stretch flex flex-row gap-2.5 h-5 items-center justify-center p-0 relative shrink-0"
      data-name="Page Title"
    >
      <div className="flex flex-col font-['Lato:Bold',_sans-serif] justify-center leading-[0] not-italic relative shrink-0 text-[#585858] text-[18px] text-left text-nowrap">
        <p className="block leading-[normal] whitespace-pre">Page Title</p>
      </div>
    </div>
  );
}

function Title() {
  return (
    <div
      className="box-border content-stretch flex flex-row gap-[3px] items-center justify-start p-0 relative shrink-0"
      data-name="Title"
    >
      <PageTitle />
      <div className="relative shrink-0 size-4" data-name="Info Icon">
        <InfoIcon />
      </div>
    </div>
  );
}

function PageSubtitle() {
  return (
    <div
      className="box-border content-stretch flex flex-row gap-2.5 items-start justify-start p-0 relative shrink-0"
      data-name="Page Subtitle"
    >
      <div className="flex flex-col font-['Lato:Regular',_sans-serif] justify-center leading-[0] not-italic relative shrink-0 text-[#585858] text-[12px] text-left text-nowrap">
        <p className="block leading-[normal] whitespace-pre">
          Last updated 12/01/2023 at 12:12 pm
        </p>
      </div>
    </div>
  );
}

function PageTitle1() {
  return (
    <div
      className="basis-0 box-border content-stretch flex flex-col gap-1 grow items-start justify-end min-h-px min-w-px p-0 relative shrink-0"
      data-name="Page Title"
    >
      <Title />
      <PageSubtitle />
    </div>
  );
}

function SaveButton() {
  return (
    <div
      className="bg-[#1b4dc0] hover:shadow-md hover:shadow-[#00000033] transition-shadow box-border content-stretch flex flex-row gap-2 h-9 items-center justify-start pl-2.5 pr-4 py-[9px] relative rounded shrink-0"
      data-name="Save Button"
    >
      <div
        className="overflow-clip relative shrink-0 size-[18px]"
        data-name="save"
      >
        <div className="absolute inset-[12.5%]" data-name="Vector">
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 14 14"
          >
            <g id="Vector">
              <path d={svgPaths.p326b05c0} fill="var(--fill-0, white)" />
            </g>
          </svg>
        </div>
      </div>
      <div className="flex flex-col font-['Lato:Regular',_sans-serif] justify-center leading-[0] not-italic relative shrink-0 text-[#ffffff] text-[14px] text-left text-nowrap">
        <p className="block leading-[normal] whitespace-pre">Save</p>
      </div>
    </div>
  );
}

function TableSettings() {
  return (
    <div
      className="group hover:bg-[#F5F5F5] box-border content-stretch flex flex-row gap-2 h-9 items-center justify-start pl-2 pr-4 py-1.5 relative rounded shrink-0 [--fill-0:#585858] group-hover:[--fill-0:#1B4DC0]"
      data-name="Table Settings"
    >
      <div
        className="overflow-clip relative shrink-0 size-6"
        data-name="table_settings"
      >
        <div
          className="absolute bottom-[3.968%] left-[2.083%] right-[1.351%] top-[12.5%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 24 21"
          >
            <g id="Vector">
              <path d={svgPaths.p31b80500} fill="var(--fill-0, #585858)" />
              <path d={svgPaths.p155baf00} fill="var(--fill-0, #585858)" />
            </g>
          </svg>
        </div>
      </div>
      <div className="flex flex-col font-['Lato:Regular',_sans-serif] justify-center leading-[0] not-italic relative shrink-0 text-[#585858] group-hover:text-[#1B4DC0] text-[14px] text-left text-nowrap">
        <p className="block leading-[normal] whitespace-pre">Table Settings</p>
      </div>
    </div>
  );
}

function OptmizeButton() {
  return (
    <div
      className="group hover:bg-[#F5F5F5] box-border content-stretch flex flex-row gap-2 h-9 items-center justify-start pl-2 pr-4 py-1.5 relative rounded shrink-0 [--fill-0:#585858] group-hover:[--fill-0:#1B4DC0]"
      data-name="Optmize Button"
    >
      <div className="overflow-clip relative shrink-0 size-6" data-name="sync">
        <div
          className="absolute bottom-[7.119%] left-[16.667%] right-[16.667%] top-[7.119%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 16 21"
          >
            <g id="Vector">
              <path d={svgPaths.p92e8700} fill="var(--fill-0, #585858)" />
            </g>
          </svg>
        </div>
      </div>
      <div className="flex flex-col font-['Lato:Regular',_sans-serif] justify-center leading-[0] not-italic relative shrink-0 text-[#585858] group-hover:text-[#1B4DC0] text-[14px] text-left text-nowrap">
        <p className="block leading-[normal] whitespace-pre">Optimize</p>
      </div>
    </div>
  );
}

function Filter() {
  return (
    <div
      className="group hover:bg-[#F5F5F5] box-border content-stretch flex flex-row items-center justify-start p-[6px] relative rounded shrink-0 [--fill-0:#585858] group-hover:[--fill-0:#1B4DC0]"
      data-name="Filter"
    >
      <div
        className="overflow-clip relative shrink-0 size-6"
        data-name="filter_alt"
      >
        <div
          className="absolute bottom-[16.667%] left-[16.827%] right-[16.827%] top-[16.667%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 16 16"
          >
            <g id="Vector">
              <path d={svgPaths.p3e89aa00} fill="var(--fill-0, #585858)" />
            </g>
          </svg>
        </div>
      </div>
    </div>
  );
}

function FilterButtonOnlyIcon() {
  return (
    <div
      className="box-border content-stretch flex flex-row items-center justify-start p-0 relative shrink-0"
      data-name="Filter Button_Only Icon"
    >
      <Filter />
    </div>
  );
}

function UploadButtonOnlyIcon() {
  return (
    <div
      className="group hover:bg-[#F5F5F5] box-border content-stretch flex flex-row items-center justify-start p-[6px] relative shrink-0 [--fill-0:#585858] group-hover:[--fill-0:#1B4DC0]"
      data-name="Upload Button_Only Icon"
    >
      <div
        className="overflow-clip relative shrink-0 size-6"
        data-name="upload"
      >
        <div
          className="absolute bottom-[15.432%] left-[20.833%] right-[20.833%] top-[15.432%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 14 17"
          >
            <g id="Vector">
              <path d={svgPaths.p18c93480} fill="var(--fill-0, #585858)" />
            </g>
          </svg>
        </div>
      </div>
    </div>
  );
}

function DownloadButtonOnlyIcon() {
  return (
    <div
      className="group hover:bg-[#F5F5F5] box-border content-stretch flex flex-row items-center justify-start p-[6px] relative rounded shrink-0 [--fill-0:#585858] group-hover:[--fill-0:#1B4DC0]"
      data-name="Download Button_Only Icon"
    >
      <div
        className="overflow-clip relative shrink-0 size-6"
        data-name="download"
      >
        <div
          className="absolute bottom-[14.583%] left-[20.833%] right-[20.833%] top-[14.583%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 14 17"
          >
            <g id="Vector">
              <path d={svgPaths.p3ea678f0} fill="var(--fill-0, #585858)" />
            </g>
          </svg>
        </div>
      </div>
    </div>
  );
}

interface ButtonsProps {
  showSaveButton: boolean;
  showTableSettings: boolean;
  showOptimizeButton: boolean;
  showFilterButton: boolean;
  showUploadButton: boolean;
  showDownloadButton: boolean;
}

function Buttons({
  showSaveButton,
  showTableSettings,
  showOptimizeButton,
  showFilterButton,
  showUploadButton,
  showDownloadButton
}: ButtonsProps) {
  // Check if we need a divider (only if there are buttons on both sides)
  const hasLeftButtons = showSaveButton || showTableSettings || showOptimizeButton;
  const hasRightButtons = showFilterButton || showUploadButton || showDownloadButton;
  const showDivider = hasLeftButtons && hasRightButtons;

  return (
    <div
      className="box-border content-stretch flex flex-row gap-2 items-center justify-end p-0 relative shrink-0"
      data-name="Buttons"
    >
      {showSaveButton && <SaveButton />}
      {showTableSettings && <TableSettings />}
      {showOptimizeButton && <OptmizeButton />}
      
      {showDivider && (
        <div
          className="box-border content-stretch flex flex-row items-start justify-start px-2 py-0 relative shrink-0"
          data-name="Page Divider"
        >
          <div className="flex h-[24px] items-center justify-center relative shrink-0 w-[0px]">
            <div className="flex-none rotate-[90deg]">
              <div className="h-0 relative w-6">
                <div
                  className="absolute bottom-0 left-0 right-0 top-[-1px]"
                  style={
                    {
                      "--stroke-0":
                        "rgba(224.000001847744, 224.000001847744, 224.000001847744, 1)",
                    } as React.CSSProperties
                  }
                >
                  <svg
                    className="block size-full"
                    fill="none"
                    preserveAspectRatio="none"
                    role="presentation"
                    viewBox="0 0 24 1"
                  >
                    <line
                      id="Line 8"
                      stroke="var(--stroke-0, #E0E0E0)"
                      x2="24"
                      y1="0.5"
                      y2="0.5"
                    />
                  </svg>
                </div>
              </div>
            </div>
          </div>
        </div>
      )}
      
      {showFilterButton && <FilterButtonOnlyIcon />}
      {showUploadButton && <UploadButtonOnlyIcon />}
      {showDownloadButton && <DownloadButtonOnlyIcon />}
    </div>
  );
}

function SearchBar() {
  const [query, setQuery] = useState("");

  return (
    <div
      className="bg-[#ffffff] box-border content-stretch flex flex-row gap-[3px] items-center justify-start pl-1.5 pr-0 py-0 relative rounded-[5px] shrink-0 w-60"
      data-name="SearchBar"
    >
      <div className="absolute border border-[#e0e0e0] border-solid inset-0 pointer-events-none rounded-[5px]" />
      <div
        className="overflow-clip relative shrink-0 size-6"
        data-name="search icon"
      >
        <div
          className="absolute bottom-[14.462%] left-[14.483%] right-[14.483%] top-[14.462%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 18 18"
          >
            <g id="Vector">
              <path d={svgPaths.p2255adf0} fill="var(--fill-0, #585858)" />
            </g>
          </svg>
        </div>
      </div>
      <input
        type="text"
        value={query}
        onChange={(e) => setQuery(e.target.value)}
        placeholder="Search"
        className="basis-0 grow h-9 min-h-px min-w-px bg-transparent outline-none font-['Lato:Regular',_sans-serif] text-[16px] text-[#1c1c1c] placeholder-[#bdbdbd] px-2"
      />
    </div>
  );
}

function DatePicker() {
  return (
    <div
      className="bg-[#ffffff] box-border content-stretch flex flex-row gap-[3px] h-9 items-center justify-start px-1.5 py-0 relative rounded-[5px] shrink-0"
      data-name="Date Picker"
    >
      <div className="absolute border border-[#e0e0e0] border-solid inset-0 pointer-events-none rounded-[5px]" />
      <div
        className="overflow-clip relative shrink-0 size-5"
        data-name="Icons/action/calendar_today_24px"
      >
        <CalendarToday style="Round" />
      </div>
      <div className="flex flex-col font-['Lato:Regular',_sans-serif] h-9 justify-center leading-[0] not-italic relative shrink-0 text-[#1c1c1c] text-[16px] text-left w-[200px]">
        <p className="block leading-[27px]">07/15/2024 – 07/31/2024</p>
      </div>
      <div
        className="overflow-clip relative shrink-0 size-5"
        data-name="Icons/action/calendar_today_24px"
      >
        <div className="absolute inset-[22.531%]" data-name="Vector">
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 11 11"
          >
            <g id="Vector">
              <path d={svgPaths.p21a6c000} fill="var(--fill-0, #1C1C1C)" />
            </g>
          </svg>
        </div>
      </div>
    </div>
  );
}

function MoreOptions() {
  return (
    <div
      className="box-border content-stretch flex flex-row items-center justify-start p-[6px] relative rounded-[5px] shrink-0 size-9"
      data-name="more options"
    >
      <div className="absolute border border-[#e0e0e0] border-solid inset-0 pointer-events-none rounded-[5px]" />
      <div
        className="overflow-clip relative shrink-0 size-6"
        data-name="more_vert"
      >
        <div
          className="absolute bottom-[16.667%] left-[41.667%] right-[41.667%] top-[16.667%]"
          data-name="Vector"
        >
          <svg
            className="block size-full"
            fill="none"
            preserveAspectRatio="none"
            role="presentation"
            viewBox="0 0 4 16"
          >
            <g id="Vector">
              <path d={svgPaths.p56f6880} fill="var(--fill-0, #585858)" />
            </g>
          </svg>
        </div>
      </div>
    </div>
  );
}

interface UtilityControlsProps {
  showButtons: boolean;
  showSearchBar: boolean;
  showSaveButton: boolean;
  showTableSettings: boolean;
  showOptimizeButton: boolean;
  showFilterButton: boolean;
  showUploadButton: boolean;
  showDownloadButton: boolean;
  showDatePicker: boolean;
  showMoreOptions: boolean;
}

function UtilityControls({
  showButtons,
  showSearchBar,
  showSaveButton,
  showTableSettings,
  showOptimizeButton,
  showFilterButton,
  showUploadButton,
  showDownloadButton,
  showDatePicker,
  showMoreOptions
}: UtilityControlsProps) {
  return (
    <div
      className="box-border content-stretch flex flex-row gap-3 items-center justify-end p-0 relative shrink-0"
      data-name="Utility Controls"
    >
      {showButtons && (
        <Buttons 
          showSaveButton={showSaveButton}
          showTableSettings={showTableSettings}
          showOptimizeButton={showOptimizeButton}
          showFilterButton={showFilterButton}
          showUploadButton={showUploadButton}
          showDownloadButton={showDownloadButton}
        />
      )}
      {showSearchBar && <SearchBar />}
      {showDatePicker && <DatePicker />}
      {showMoreOptions && <MoreOptions />}
    </div>
  );
}

interface TopOfPageProps {
  showButtons?: boolean;
  showSearchBar?: boolean;
  showSaveButton?: boolean;
  showTableSettings?: boolean;
  showOptimizeButton?: boolean;
  showFilterButton?: boolean;
  showUploadButton?: boolean;
  showDownloadButton?: boolean;
  showDatePicker?: boolean;
  showMoreOptions?: boolean;
}

export default function TopOfPage({
  showButtons = true,
  showSearchBar = true,
  showSaveButton = true,
  showTableSettings = true,
  showOptimizeButton = true,
  showFilterButton = true,
  showUploadButton = true,
  showDownloadButton = true,
  showDatePicker = true,
  showMoreOptions = true
}: TopOfPageProps) {
  return (
    <div className="bg-[#ffffff] relative size-full" data-name="Top of Page">
      <div className="absolute border-[#eeeeee] border-[0px_0px_1px] border-solid inset-0 pointer-events-none" />
      <div className="flex flex-row items-center relative size-full">
        <div className="box-border content-stretch flex flex-row items-center justify-start px-6 py-1 relative size-full">
          <PageTitle1 />
          <UtilityControls 
            showButtons={showButtons}
            showSearchBar={showSearchBar}
            showSaveButton={showSaveButton}
            showTableSettings={showTableSettings}
            showOptimizeButton={showOptimizeButton}
            showFilterButton={showFilterButton}
            showUploadButton={showUploadButton}
            showDownloadButton={showDownloadButton}
            showDatePicker={showDatePicker}
            showMoreOptions={showMoreOptions}
          />
        </div>
      </div>
    </div>
  );
}

defineProperties(TopOfPage, {
  showButtons: {
    label: "Show All Buttons",
    type: "boolean",
    defaultValue: true,
  },
  showSearchBar: {
    label: "Show Search Bar",
    type: "boolean",
    defaultValue: true,
  },
  showSaveButton: {
    label: "Show Save Button",
    type: "boolean",
    defaultValue: true,
  },
  showTableSettings: {
    label: "Show Table Settings Button",
    type: "boolean",
    defaultValue: true,
  },
  showOptimizeButton: {
    label: "Show Optimize Button",
    type: "boolean",
    defaultValue: true,
  },
  showFilterButton: {
    label: "Show Filter Button",
    type: "boolean",
    defaultValue: true,
  },
  showUploadButton: {
    label: "Show Upload Button",
    type: "boolean",
    defaultValue: true,
  },
  showDownloadButton: {
    label: "Show Download Button",
    type: "boolean",
    defaultValue: true,
  },
  showDatePicker: {
    label: "Show Date Picker",
    type: "boolean",
    defaultValue: true,
  },
  showMoreOptions: {
    label: "Show More Options Menu",
    type: "boolean",
    defaultValue: true,
  }
});

this is the missing svg path, create a .ts file and import it:

export default {
p155baf00: "M22.1127 15.2668C22.1127 15.1569 22.108 15.0517 22.0984 14.9417L22.9876 14.2676C23.1789 14.1242 23.2315 13.8565 23.1119 13.6461L22.2179 12.1019C22.0984 11.8915 21.8402 11.8055 21.6203 11.9011L20.5924 12.3362C20.4155 12.2119 20.2291 12.1019 20.0331 12.0111L19.8944 10.9067C19.8657 10.6676 19.6602 10.486 19.4211 10.486H17.6378C17.394 10.486 17.1884 10.6676 17.1598 10.9067L17.0211 12.0111C16.8251 12.1019 16.6386 12.2119 16.4618 12.3362L15.4339 11.9011C15.2139 11.8055 14.9558 11.8915 14.8363 12.1019L13.9422 13.6509C13.8227 13.8613 13.8753 14.1242 14.0665 14.2724L14.9558 14.9465C14.9462 15.0517 14.9414 15.1569 14.9414 15.2668C14.9414 15.3768 14.9462 15.482 14.9558 15.5919L14.0665 16.266C13.8753 16.4095 13.8227 16.6772 13.9422 16.8876L14.8363 18.4318C14.9558 18.6421 15.2139 18.7282 15.4339 18.6326L16.4618 18.1975C16.6386 18.3218 16.8251 18.4318 17.0211 18.5226L17.1598 19.627C17.1884 19.866 17.394 20.0477 17.6331 20.0477H19.4163C19.6554 20.0477 19.861 19.866 19.8896 19.627L20.0283 18.5226C20.2243 18.4318 20.4108 18.3218 20.5876 18.1975L21.6155 18.6326C21.8355 18.7282 22.0936 18.6421 22.2131 18.4318L23.1072 16.8876C23.2267 16.6772 23.1741 16.4142 22.9829 16.266L22.0936 15.5919C22.108 15.482 22.1127 15.3768 22.1127 15.2668ZM18.5462 16.9401C17.6235 16.9401 16.8729 16.1895 16.8729 15.2668C16.8729 14.3441 17.6235 13.5935 18.5462 13.5935C19.4689 13.5935 20.2195 14.3441 20.2195 15.2668C20.2195 16.1895 19.4689 16.9401 18.5462 16.9401Z",
p18c93480: "M5 12.5925H9C9.55 12.5925 10 12.1425 10 11.5925V6.5925H11.59C12.48 6.5925 12.93 5.5125 12.3 4.8825L7.71 0.2925C7.32 -0.0975 6.69 -0.0975 6.3 0.2925L1.71 4.8825C1.08 5.5125 1.52 6.5925 2.41 6.5925H4V11.5925C4 12.1425 4.45 12.5925 5 12.5925ZM1 14.5925H13C13.55 14.5925 14 15.0425 14 15.5925C14 16.1425 13.55 16.5925 13 16.5925H1C0.45 16.5925 0 16.1425 0 15.5925C0 15.0425 0.45 14.5925 1 14.5925Z",
p1e3c3180: "M20 2H17V0H15V2H5V0H3V2H0V22H20V2ZM18 20H2V7H18V20Z",
p21a6c000: "M10.7437 0.252084C10.4187 -0.0729165 9.89375 -0.0729165 9.56875 0.252084L5.49375 4.31875L1.41875 0.24375C1.09375 -0.08125 0.56875 -0.08125 0.24375 0.24375C-0.08125 0.56875 -0.08125 1.09375 0.24375 1.41875L4.31875 5.49375L0.24375 9.56875C-0.08125 9.89375 -0.08125 10.4187 0.24375 10.7437C0.56875 11.0687 1.09375 11.0687 1.41875 10.7437L5.49375 6.66875L9.56875 10.7437C9.89375 11.0687 10.4187 11.0687 10.7437 10.7437C11.0687 10.4187 11.0687 9.89375 10.7437 9.56875L6.66875 5.49375L10.7437 1.41875C11.0604 1.10208 11.0604 0.56875 10.7437 0.252084Z",
p2255adf0: "M12.5006 11.0006H11.7106L11.4306 10.7306C12.6306 9.33063 13.2506 7.42063 12.9106 5.39063C12.4406 2.61063 10.1206 0.390626 7.32063 0.0506256C3.09063 -0.469374 -0.469374 3.09063 0.0506256 7.32063C0.390626 10.1206 2.61063 12.4406 5.39063 12.9106C7.42063 13.2506 9.33063 12.6306 10.7306 11.4306L11.0006 11.7106V12.5006L15.2506 16.7506C15.6606 17.1606 16.3306 17.1606 16.7406 16.7506C17.1506 16.3406 17.1506 15.6706 16.7406 15.2606L12.5006 11.0006ZM6.50063 11.0006C4.01063 11.0006 2.00063 8.99063 2.00063 6.50063C2.00063 4.01063 4.01063 2.00063 6.50063 2.00063C8.99063 2.00063 11.0006 4.01063 11.0006 6.50063C11.0006 8.99063 8.99063 11.0006 6.50063 11.0006Z",
p23caf740: "M18 2H17V1C17 0.45 16.55 0 16 0C15.45 0 15 0.45 15 1V2H5V1C5 0.45 4.55 0 4 0C3.45 0 3 0.45 3 1V2H2C0.9 2 0 2.9 0 4V20C0 21.1 0.9 22 2 22H18C19.1 22 20 21.1 20 20V4C20 2.9 19.1 2 18 2ZM17 20H3C2.45 20 2 19.55 2 19V7H18V19C18 19.55 17.55 20 17 20Z",
p264aa300: "M18 2H17V0H15V2H5V0H3V2H2C0.9 2 0 2.9 0 4V20C0 21.1 0.9 22 2 22H18C19.1 22 20 21.1 20 20V4C20 2.9 19.1 2 18 2ZM18 4V7H2V4H18ZM2 20V9H18V20H2Z",
p30b72580: "M18 2H17V0H15V2H5V0H3V2H2C0.9 2 0 2.9 0 4V20C0 21.1 0.9 22 2 22H18C19.1 22 20 21.1 20 20V4C20 2.9 19.1 2 18 2ZM18 20H2V9H18V20ZM18 7H2V4H18V7Z",
p31b80500: "M7 7.02H12V18H7V7.02ZM14 8.51H19V7H14V8.51ZM17 0H2C0.9 0 0 0.9 0 2V5H19V2C19 0.9 18.1 0 17 0ZM0 16C0 17.1 0.9 18 2 18H5V7H0V16Z",
p326b05c0: "M10.9425 0.4425C10.6575 0.1575 10.275 0 9.8775 0H1.5C0.6675 0 0 0.675 0 1.5V12C0 12.825 0.675 13.5 1.5 13.5H12C12.825 13.5 13.5 12.825 13.5 12V3.6225C13.5 3.225 13.3425 2.8425 13.0575 2.565L10.9425 0.4425ZM6.75 12C5.505 12 4.5 10.995 4.5 9.75C4.5 8.505 5.505 7.5 6.75 7.5C7.995 7.5 9 8.505 9 9.75C9 10.995 7.995 12 6.75 12ZM7.5 4.5H3C2.175 4.5 1.5 3.825 1.5 3C1.5 2.175 2.175 1.5 3 1.5H7.5C8.325 1.5 9 2.175 9 3C9 3.825 8.325 4.5 7.5 4.5Z",
p36026d80: "M18 2H17V0H15V2H5V0H3V2H2C0.9 2 0 2.9 0 4V20C0 21.1 0.9 22 2 22H18C19.1 22 20 21.1 20 20V4C20 2.9 19.1 2 18 2ZM18 20H2V7H18V20Z",
p3e89aa00: "M0.211604 1.61C2.5316 4.59 5.9616 9 5.9616 9V14C5.9616 15.1 6.8616 16 7.9616 16C9.0616 16 9.9616 15.1 9.9616 14V9C9.9616 9 13.3916 4.59 15.7116 1.61C16.2216 0.95 15.7516 0 14.9116 0H1.0016C0.171604 0 -0.298396 0.95 0.211604 1.61Z",
p3ea678f0: "M11.59 6H10V1C10 0.45 9.55 0 9 0H5C4.45 0 4 0.45 4 1V6H2.41C1.52 6 1.07 7.08 1.7 7.71L6.29 12.3C6.68 12.69 7.31 12.69 7.7 12.3L12.29 7.71C12.92 7.08 12.48 6 11.59 6ZM0 16C0 16.55 0.45 17 1 17H13C13.55 17 14 16.55 14 16C14 15.45 13.55 15 13 15H1C0.45 15 0 15.45 0 16Z",
p56f6880: "M2 4C3.1 4 4 3.1 4 2C4 0.9 3.1 0 2 0C0.9 0 0 0.9 0 2C0 3.1 0.9 4 2 4ZM2 6C0.9 6 0 6.9 0 8C0 9.1 0.9 10 2 10C3.1 10 4 9.1 4 8C4 6.9 3.1 6 2 6ZM2 12C0.9 12 0 12.9 0 14C0 15.1 0.9 16 2 16C3.1 16 4 15.1 4 14C4 12.9 3.1 12 2 12Z",
p92e8700: "M8 2.29153V0.501534C8 0.0515344 7.46 -0.168466 7.15 0.151534L4.35 2.94153C4.15 3.14153 4.15 3.45153 4.35 3.65153L7.14 6.44153C7.46 6.75153 8 6.53153 8 6.08153V4.29153C11.31 4.29153 14 6.98153 14 10.2915C14 11.0815 13.85 11.8515 13.56 12.5415C13.41 12.9015 13.52 13.3115 13.79 13.5815C14.3 14.0915 15.16 13.9115 15.43 13.2415C15.8 12.3315 16 11.3315 16 10.2915C16 5.87153 12.42 2.29153 8 2.29153ZM8 16.2915C4.69 16.2915 2 13.6015 2 10.2915C2 9.50153 2.15 8.73153 2.44 8.04153C2.59 7.68153 2.48 7.27153 2.21 7.00153C1.7 6.49153 0.84 6.67153 0.57 7.34153C0.2 8.25153 0 9.25153 0 10.2915C0 14.7115 3.58 18.2915 8 18.2915V20.0815C8 20.5315 8.54 20.7515 8.85 20.4315L11.64 17.6415C11.84 17.4415 11.84 17.1315 11.64 16.9315L8.85 14.1415C8.54 13.8315 8 14.0515 8 14.5015V16.2915Z",
pa266500: "M7.5 0C3.36 0 0 3.36 0 7.5C0 11.64 3.36 15 7.5 15C11.64 15 15 11.64 15 7.5C15 3.36 11.64 0 7.5 0ZM8.25 11.25H6.75V6.75H8.25V11.25ZM8.25 5.25H6.75V3.75H8.25V5.25Z",
}
```
